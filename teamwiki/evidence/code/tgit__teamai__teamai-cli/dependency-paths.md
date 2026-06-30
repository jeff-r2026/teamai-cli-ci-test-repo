---
title: tgit__teamai__teamai-cli dependency paths
domain: code-knowledge
---

# Dependency Paths

Static import dependency paths (not runtime call traces).

18 dependency path(s) traced from entry points (max depth 4).

## buildHandlerRegistry (src/hook-handlers.ts)

- [entry] `buildHandlerRegistry` ← src/hook-handlers.ts:235
  - [orchestration] `createDispatcher` ← src/hook-dispatch.ts:235
    - [service] `deriveSessionId` ← src/utils/session-id.ts:235
    - [service] `normalizeToolName` ← src/utils/tool-names.ts:235
    - [service] `filterRulesByKnowledgeNamespaces` ← src/pull.ts:235
    - [service] `loadTeamConfig` ← src/config.ts:235
    - [service] `expandHome` ← src/utils/fs.ts:235
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:235
    - [service] `loadRolesManifest` ← src/roles.ts:235
    - [service] `extractToml` ← src/wiki-engine/code-knowledge/extractors/config.ts:235
    - [service] `isKeyFile` ← src/wiki-engine/code-knowledge/code-collector.ts:235
    - [service] `mapKindToEvidenceType` ← src/wiki-engine/code-knowledge/code-extractors.ts:235
    - [service] `createGit` ← src/utils/git.ts:235
    - [service] `injectClaudeMdSection` ← src/utils/claudemd.ts:235
    - [service] `resolveRegistryForPackage` ← src/update.ts:235
    - [service] `resolveEffectiveUpdatePolicy` ← src/update-policy.ts:235
      - [data] `ToolPathsSchema` ← src/types.ts:235
    - [service] `RepoNotFoundError` ← src/providers/types.ts:235

## EndpointMap (src/status-report.ts)

- [entry] `EndpointMap` ← src/status-report.ts:38
    - [service] `loadTeamConfig` ← src/config.ts:38
    - [service] `expandHome` ← src/utils/fs.ts:38
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:38
    - [service] `loadRolesManifest` ← src/roles.ts:38
    - [service] `extractToml` ← src/wiki-engine/code-knowledge/extractors/config.ts:38
    - [service] `isKeyFile` ← src/wiki-engine/code-knowledge/code-collector.ts:38
    - [service] `safeIgnore` ← src/wiki-engine/core/wiki-protocol.ts:38
    - [service] `mapKindToEvidenceType` ← src/wiki-engine/code-knowledge/code-extractors.ts:38
    - [service] `getApiKeyPath` ← src/api-key.ts:38
  - [orchestration] `installSkillZip` ← src/skill-command.ts:38
    - [service] `assertSafePath` ← src/utils/path-safety.ts:38
      - [data] `ToolPathsSchema` ← src/types.ts:38
    - [service] `RepoNotFoundError` ← src/providers/types.ts:38
    - [service] `getMachineId` ← src/machine-id.ts:38

## resolveEndpoints (src/status-report.ts)

- [entry] `resolveEndpoints` ← src/status-report.ts:56
    - [service] `loadTeamConfig` ← src/config.ts:56
    - [service] `expandHome` ← src/utils/fs.ts:56
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:56
    - [service] `loadRolesManifest` ← src/roles.ts:56
    - [service] `extractToml` ← src/wiki-engine/code-knowledge/extractors/config.ts:56
    - [service] `isKeyFile` ← src/wiki-engine/code-knowledge/code-collector.ts:56
    - [service] `safeIgnore` ← src/wiki-engine/core/wiki-protocol.ts:56
    - [service] `mapKindToEvidenceType` ← src/wiki-engine/code-knowledge/code-extractors.ts:56
    - [service] `getApiKeyPath` ← src/api-key.ts:56
  - [orchestration] `installSkillZip` ← src/skill-command.ts:56
    - [service] `assertSafePath` ← src/utils/path-safety.ts:56
      - [data] `ToolPathsSchema` ← src/types.ts:56
    - [service] `RepoNotFoundError` ← src/providers/types.ts:56
    - [service] `getMachineId` ← src/machine-id.ts:56

## resolveReportEndpoint (src/status-report.ts)

- [entry] `resolveReportEndpoint` ← src/status-report.ts:90
    - [service] `loadTeamConfig` ← src/config.ts:90
    - [service] `expandHome` ← src/utils/fs.ts:90
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:90
    - [service] `loadRolesManifest` ← src/roles.ts:90
    - [service] `extractToml` ← src/wiki-engine/code-knowledge/extractors/config.ts:90
    - [service] `isKeyFile` ← src/wiki-engine/code-knowledge/code-collector.ts:90
    - [service] `safeIgnore` ← src/wiki-engine/core/wiki-protocol.ts:90
    - [service] `mapKindToEvidenceType` ← src/wiki-engine/code-knowledge/code-extractors.ts:90
    - [service] `getApiKeyPath` ← src/api-key.ts:90
  - [orchestration] `installSkillZip` ← src/skill-command.ts:90
    - [service] `assertSafePath` ← src/utils/path-safety.ts:90
      - [data] `ToolPathsSchema` ← src/types.ts:90
    - [service] `RepoNotFoundError` ← src/providers/types.ts:90
    - [service] `getMachineId` ← src/machine-id.ts:90

## getHandler (src/resources/index.ts)

- [entry] `getHandler` ← src/resources/index.ts:21
- [entry] `ResourceHandler` ← src/resources/base.ts:21
      - [data] `ToolPathsSchema` ← src/types.ts:21
    - [service] `RepoNotFoundError` ← src/providers/types.ts:21
    - [service] `expandHome` ← src/utils/fs.ts:21
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:21
    - [service] `ensureSkillFrontmatter` ← src/resources/skills.ts:21
- [entry] `RulesHandler` ← src/resources/rules.ts:21
- [entry] `DocsHandler` ← src/resources/docs.ts:21
- [entry] `EnvHandler` ← src/resources/env.ts:21

## getAllHandlers (src/resources/index.ts)

- [entry] `getAllHandlers` ← src/resources/index.ts:25
- [entry] `ResourceHandler` ← src/resources/base.ts:25
      - [data] `ToolPathsSchema` ← src/types.ts:25
    - [service] `RepoNotFoundError` ← src/providers/types.ts:25
    - [service] `expandHome` ← src/utils/fs.ts:25
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:25
    - [service] `ensureSkillFrontmatter` ← src/resources/skills.ts:25
- [entry] `RulesHandler` ← src/resources/rules.ts:25
- [entry] `DocsHandler` ← src/resources/docs.ts:25
- [entry] `EnvHandler` ← src/resources/env.ts:25

## AgentsHandler (src/resources/agents.ts)

- [entry] `AgentsHandler` ← src/resources/agents.ts:43
- [entry] `ResourceHandler` ← src/resources/base.ts:43
      - [data] `ToolPathsSchema` ← src/types.ts:43
    - [service] `RepoNotFoundError` ← src/providers/types.ts:43
    - [service] `expandHome` ← src/utils/fs.ts:43
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:43

## DocsHandler (src/resources/docs.ts)

- [entry] `DocsHandler` ← src/resources/docs.ts:9
- [entry] `ResourceHandler` ← src/resources/base.ts:9
      - [data] `ToolPathsSchema` ← src/types.ts:9
    - [service] `RepoNotFoundError` ← src/providers/types.ts:9
    - [service] `expandHome` ← src/utils/fs.ts:9
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:9

## EnvHandler (src/resources/env.ts)

- [entry] `EnvHandler` ← src/resources/env.ts:37
- [entry] `ResourceHandler` ← src/resources/base.ts:37
      - [data] `ToolPathsSchema` ← src/types.ts:37
    - [service] `RepoNotFoundError` ← src/providers/types.ts:37
    - [service] `expandHome` ← src/utils/fs.ts:37
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:37

## HooksHandler (src/resources/hooks.ts)

- [entry] `HooksHandler` ← src/resources/hooks.ts:168
- [entry] `ResourceHandler` ← src/resources/base.ts:168
      - [data] `ToolPathsSchema` ← src/types.ts:168
    - [service] `RepoNotFoundError` ← src/providers/types.ts:168
    - [service] `expandHome` ← src/utils/fs.ts:168
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:168

## RulesHandler (src/resources/rules.ts)

- [entry] `RulesHandler` ← src/resources/rules.ts:10
- [entry] `ResourceHandler` ← src/resources/base.ts:10
      - [data] `ToolPathsSchema` ← src/types.ts:10
    - [service] `RepoNotFoundError` ← src/providers/types.ts:10
    - [service] `expandHome` ← src/utils/fs.ts:10
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:10

## SkillsHandler (src/resources/skills.ts)

- [entry] `SkillsHandler` ← src/resources/skills.ts:207
- [entry] `ResourceHandler` ← src/resources/base.ts:207
      - [data] `ToolPathsSchema` ← src/types.ts:207
    - [service] `RepoNotFoundError` ← src/providers/types.ts:207
    - [service] `expandHome` ← src/utils/fs.ts:207
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:207

## WikiHandler (src/resources/wiki.ts)

- [entry] `WikiHandler` ← src/resources/wiki.ts:35
- [entry] `ResourceHandler` ← src/resources/base.ts:35
      - [data] `ToolPathsSchema` ← src/types.ts:35
    - [service] `RepoNotFoundError` ← src/providers/types.ts:35
    - [service] `expandHome` ← src/utils/fs.ts:35
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:35

## ResourceHandler (src/resources/base.ts)

- [entry] `ResourceHandler` ← src/resources/base.ts:11
      - [data] `ToolPathsSchema` ← src/types.ts:11
    - [service] `RepoNotFoundError` ← src/providers/types.ts:11
    - [service] `expandHome` ← src/utils/fs.ts:11
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:11

## handler (src/openclaw-hooks.ts)

- [entry] `handler` ← src/openclaw-hooks.ts:60
    - [service] `expandHome` ← src/utils/fs.ts:60
    - [service] `MAX_LOG_BYTES` ← src/utils/logger.ts:60

## HookHandler (src/hook-dispatch.ts)

- [entry] `HookHandler` ← src/hook-dispatch.ts:16

## HandlerRegistration (src/hook-dispatch.ts)

- [entry] `HandlerRegistration` ← src/hook-dispatch.ts:21

## routerTemplate (src/wiki-engine/adapters/templates.ts)

- [entry] `routerTemplate` ← src/wiki-engine/adapters/templates.ts:7
