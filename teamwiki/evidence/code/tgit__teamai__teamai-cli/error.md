---
title: tgit__teamai__teamai-cli error
domain: code-knowledge
source:
  - src/providers/github/index.ts
  - src/dashboard-collector.ts
  - src/enrich-with-ai.ts
  - src/source-http.ts
  - src/utils/ai-client.ts
---

# Error

- `RepoNotFoundError` ← src/providers/github/index.ts:44 [EXTRACTED]
  ```
  throw new RepoNotFoundError(repo);
  ```
- `TRANSCRIPT_INTERRUPT_PREFIX` ← src/dashboard-collector.ts:19 [INFERRED]
  ```
  TRANSCRIPT_INTERRUPT_PREFIX,
  ```
- `INFERRED` ← src/enrich-with-ai.ts:150 [INFERRED]
  ```
  confidence: 'INFERRED' as const,
  ```
- `RepoNotAvailableError` ← src/source-http.ts:63 [EXTRACTED]
  ```
  throw new RepoNotAvailableError(`/repo not available yet (HTTP 404) at ${url}`);
  ```
- `AggregateError` ← src/utils/ai-client.ts:204 [EXTRACTED]
  ```
  throw new AggregateError(errors, `${errors.length} AI task(s) failed`);
  ```