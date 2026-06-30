---
title: tgit__teamai__teamai-cli — src module
domain: code-knowledge
source: [src/]
---

# src

**811 facts** (component: 566, interface: 214, config: 26, error: 5)

**Depends on**: tsup.config.ts

## Core components

- `ConfidenceFactor` ← src/wiki-engine/reconciler-v2-types.ts:5 (92 refs)
- `NumericConfidence` ← src/wiki-engine/reconciler-v2-types.ts:11 (92 refs)
- `fromLegacyConfidence` ← src/wiki-engine/reconciler-v2-types.ts:18 (92 refs)
- `labelFromScore` ← src/wiki-engine/reconciler-v2-types.ts:32 (92 refs)
- `buildConfidence` ← src/wiki-engine/reconciler-v2-types.ts:39 (92 refs)
- `ApiInterfaceMatch` ← src/wiki-engine/reconciler-v2-types.ts:48 (92 refs)
- `RuleCodeMatch` ← src/wiki-engine/reconciler-v2-types.ts:58 (92 refs)
- `ReconcileStaleWarning` ← src/wiki-engine/reconciler-v2-types.ts:67 (92 refs)
- `ReconcileLogEntry` ← src/wiki-engine/reconciler-v2-types.ts:78 (92 refs)
- `ReconcileStats` ← src/wiki-engine/reconciler-v2-types.ts:94 (92 refs)
- `ReconcileV2Extensions` ← src/wiki-engine/reconciler-v2-types.ts:109 (92 refs)
- `extractTypescript` ← src/wiki-engine/code-knowledge/extractors/typescript.ts:8 (92 refs)
- `RepoInfo` ← src/providers/types.ts:17 (91 refs)
- `PrCreateOptions` ← src/providers/types.ts:25 (91 refs)
- `OrgRepoInfo` ← src/providers/types.ts:45 (91 refs)
- `GitProvider` ← src/providers/types.ts:62 (91 refs)
- `RepoNotFoundError` ← src/providers/types.ts:144 (91 refs)
- `ToolPathsSchema` ← src/types.ts:6 (90 refs)
- `ScopeEnum` ← src/types.ts:19 (90 refs)
- `Scope` ← src/types.ts:20 (90 refs)

## Config

- `process.env.TEAMAI_CACHE_DIR` ← src/utils/cache-index.ts
- `process.env.TEAMAI_CACHE_MAX_BYTES` ← src/utils/cache-index.ts
- `process.env.HOME` ← src/utils/search-index.ts
- `process.env.TEAMAI_API_TOKEN` ← src/api-key.ts
- `process.env.TEAMAI_RECALL_DISABLED` ← src/auto-recall.ts
- `process.env.TEAMAI_EVAL_LOG_PATH` ← src/auto-recall.ts
- `process.env.TEAMAI_SEARCH_STRATEGY` ← src/auto-recall.ts
- `process.env.CLAUDE_SESSION_ID` ← src/contribute-check.ts
- `process.env.SHELL` ← src/doctor.ts
- `process.env.TEAMAI_MR_HINT_DISABLED` ← src/mr-hint.ts

## Errors

- `RepoNotFoundError` ← src/providers/github/index.ts
- `TRANSCRIPT_INTERRUPT_PREFIX` ← src/dashboard-collector.ts
- `INFERRED` ← src/enrich-with-ai.ts
- `RepoNotAvailableError` ← src/source-http.ts
- `AggregateError` ← src/utils/ai-client.ts
