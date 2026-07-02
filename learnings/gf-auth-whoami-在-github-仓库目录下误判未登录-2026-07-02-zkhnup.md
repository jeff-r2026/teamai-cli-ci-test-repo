---
title: "gf auth whoami 在 GitHub 仓库目录下误判未登录"
author: jeffyxu
date: 2026-07-02
tags: [gf-cli, tgit, authentication, netrc, troubleshooting]
---

# gf auth whoami 在 GitHub 仓库目录下误判未登录

## 问题现象

运行 `teamai init --repo https://git.woa.com/teamai/teamai-dev-repo` 时，选择"通过 iOA 快速登录"后报 "登录异常 / Authentication failed"。即使 token 实际有效（curl 直接调用 API 能返回用户信息），`gf auth whoami` 仍然报"未登录"。

## 根因分析

gf CLI 内部的 `vars.host()` 函数按以下优先级确定目标 host：

1. 环境变量 `GONGFENG_HOST`
2. 当前目录 git repo 的 remote URL 中解析出的 host
3. 兜底值 `git.woa.com`

当用户在一个 remote 为 `github.com` 的仓库目录（如 teamai-cli）中运行 gf 命令时，`vars.host()` 解析出 `github.com`，然后去 `~/.netrc` 中查找 `github.com` 对应的凭据。由于 netrc 中只有 `git.woa.com` 的 token，查找失败，导致报"未登录"。

## 解决方案

以下任一方式均可规避：

1. **在 home 目录或非 git 仓库目录下运行**：
   ```bash
   cd ~ && teamai init --repo https://git.woa.com/teamai/teamai-dev-repo
   ```

2. **在 git.woa.com 的仓库目录下运行**：gf 会正确解析出 `git.woa.com`。

3. **设置环境变量**（最可靠）：
   ```bash
   export GONGFENG_HOST=git.woa.com
   teamai init --repo https://git.woa.com/teamai/teamai-dev-repo
   ```

## 排查路径（供后续参考）

| 步骤 | 操作 | 结论 |
|------|------|------|
| 1 | 检查代理配置 | 无代理，排除网络问题 |
| 2 | 检查 iOA 进程 | 正常运行 |
| 3 | curl 直接调用 API | token 有效，返回用户信息 |
| 4 | 检查 ~/.netrc | 文件存在且内容正确 |
| 5 | 分析 gf CLI 源码 | 发现 vars.host() 的优先级逻辑 |
| 6 | 在 home 目录重试 | 认证成功，确认根因 |

## 关键收获

- gf CLI 的认证与**当前工作目录**强耦合，不仅仅依赖 netrc 文件是否存在。
- 当排查"token 有效但 CLI 报未登录"时，优先检查 CLI 的 host 解析逻辑。
- `~/.netrc` 的 machine 字段必须与 CLI 实际查找的 host 匹配。
