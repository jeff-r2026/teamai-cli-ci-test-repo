---
title: tgit__teamai__teamai-cli overview
domain: code-knowledge
---

# tgit__teamai__teamai-cli

**1478 facts** extracted from 158 files.
Graph: 820 nodes, 1034 edges.

## Module Structure

| Module | Facts | Components | Interfaces |
|--------|-------|------------|------------|
| src | 811 | 566 | 214 |

## Dependencies

- **src** → tsup.config.ts

## Key Dependency Paths

- buildHandlerRegistry (src/hook-handlers.ts): buildHandlerRegistry → createDispatcher → deriveSessionId → normalizeToolName → filterRulesByKnowledgeNamespaces → loadTeamConfig → expandHome → MAX_LOG_BYTES → loadRolesManifest → extractToml → isKeyFile → mapKindToEvidenceType → createGit → injectClaudeMdSection → resolveRegistryForPackage → resolveEffectiveUpdatePolicy → ToolPathsSchema → RepoNotFoundError
- EndpointMap (src/status-report.ts): EndpointMap → loadTeamConfig → expandHome → MAX_LOG_BYTES → loadRolesManifest → extractToml → isKeyFile → safeIgnore → mapKindToEvidenceType → getApiKeyPath → installSkillZip → assertSafePath → ToolPathsSchema → RepoNotFoundError → getMachineId
- resolveEndpoints (src/status-report.ts): resolveEndpoints → loadTeamConfig → expandHome → MAX_LOG_BYTES → loadRolesManifest → extractToml → isKeyFile → safeIgnore → mapKindToEvidenceType → getApiKeyPath → installSkillZip → assertSafePath → ToolPathsSchema → RepoNotFoundError → getMachineId
- resolveReportEndpoint (src/status-report.ts): resolveReportEndpoint → loadTeamConfig → expandHome → MAX_LOG_BYTES → loadRolesManifest → extractToml → isKeyFile → safeIgnore → mapKindToEvidenceType → getApiKeyPath → installSkillZip → assertSafePath → ToolPathsSchema → RepoNotFoundError → getMachineId
- getHandler (src/resources/index.ts): getHandler → ResourceHandler → ToolPathsSchema → RepoNotFoundError → expandHome → MAX_LOG_BYTES → ensureSkillFrontmatter → RulesHandler → DocsHandler → EnvHandler
