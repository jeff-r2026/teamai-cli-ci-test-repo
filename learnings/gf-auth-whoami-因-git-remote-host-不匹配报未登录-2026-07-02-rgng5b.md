---
title: "gf auth whoami 因 git remote host 不匹配报未登录"
author: jeffyxu
date: 2026-07-02
tags: [gf-cli, troubleshooting, authentication, config]
---

## 背景
运行 `teamai init` 时，gf auth login 通过 iOA 登录失败。排查发现不是代理/网络问题，token 实际有效但 gf CLI 报"还未登录"。

## 根因
`gf auth whoami` 内部调用 `vars.host()` 确定要查询的 netrc machine。该函数的优先级：
1. 环境变量 `GONGFENG_HOST`
2. 当前目录 git remote 的 host（`git remote get-url origin` → URL.host）
3. 默认值 `git.woa.com`

在 github.com 托管的仓库目录下运行时，`vars.host()` 返回 `github.com`，导致 netrc-parser 去查 `github.com` 条目（无 login），判定为未登录。

## 解决方案
1. 确保 `~/.netrc` 存在且包含 `git.woa.com` 的凭据（标准多行 netrc 格式）
2. 运行 `teamai init` 或 `gf auth whoami` 时，切换到非 github.com remote 的目录：
   ```bash
   cd ~ && teamai init --repo https://git.woa.com/teamai/teamai-dev-repo
   ```
3. 或者设置环境变量强制指定 host：
   ```bash
   GONGFENG_HOST=git.woa.com gf auth whoami
   ```

## 经验总结
- gf CLI 的认证状态是**目录敏感**的，不同目录下可能返回不同结果
- `~/.netrc` 被删除后需要重建，gf 不会自动从 macOS Keychain 恢复
- iOA 登录失败时，优先用"通过浏览器登录"或 `--token` 方式（需 personal access token）
- 排查 gf 认证问题时，可用 `node -e` 直接调用 netrc-parser 验证文件是否可读

## 相关 Skills
- teamai-recall
