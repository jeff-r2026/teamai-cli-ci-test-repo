---
title: tgit__teamai__teamai-cli interface
domain: code-knowledge
source:
  - src/utils/cache-index.ts
  - src/utils/search-index.ts
  - src/agent-skills.ts
  - src/aggregate.ts
  - src/auto-recall.ts
  - src/builtin-hooks.ts
  - src/cache-cmd.ts
  - src/clone.ts
  - src/code-knowledge-recall.ts
  - src/codebase-cmd.ts
  - src/codebase-extract.ts
  - src/codebase-lint.ts
  - src/codebase-upgrade-wiki.ts
  - src/codebase-wiki-lint.ts
  - src/deep-enrich.ts
  - src/digest.ts
  - src/drift-cmd.ts
  - src/enrich-with-ai.ts
  - src/hook-dispatch.ts
  - src/hooks.ts
  - src/import-org.ts
  - src/import-repo-list.ts
  - src/import-repo.ts
  - src/iwiki-dual.ts
  - src/known-agents.ts
  - src/mr-hint.ts
  - src/review-cmd.ts
  - src/review-store.ts
  - src/roles.ts
  - src/section-patcher.ts
  - src/skill-command.ts
  - src/source-http.ts
  - src/status-report.ts
  - src/status.ts
  - src/types.ts
  - src/update-policy.ts
  - src/update.ts
  - src/ci/extract-mr.ts
  - src/ci/mr-comment.ts
  - src/ci/read-rejections.ts
  - src/domains/recommend.ts
  - src/domains/review.ts
  - src/domains/schema.ts
  - src/providers/types.ts
  - src/repo-list/schema.ts
  - src/resources/agent-format.ts
  - src/resources/agents.ts
  - src/resources/env.ts
  - src/resources/hooks.ts
  - src/utils/iwiki-client.ts
  - src/utils/session-id.ts
  - src/utils/source-conflict.ts
  - src/utils/team-codebase-paths.ts
  - src/wiki-engine/call-chain-tracer.ts
  - src/wiki-engine/doc-graph-extractor.ts
  - src/wiki-engine/interface-scanner.ts
  - src/wiki-engine/knowledge-reconciler.ts
  - src/wiki-engine/manifest-compiler.ts
  - src/wiki-engine/manifest-schema.ts
  - src/wiki-engine/reconciler-v2-types.ts
  - src/providers/github/gh-cli.ts
  - src/providers/tgit/gf-cli.ts
  - src/wiki-engine/adapters/templates.ts
  - src/wiki-engine/code-knowledge/code-collector.ts
  - src/wiki-engine/code-knowledge/code-extractors.ts
  - src/wiki-engine/code-knowledge/code-graph.ts
  - src/wiki-engine/code-knowledge/code-incremental.ts
  - src/wiki-engine/core/graph-index.schema.ts
  - src/wiki-engine/core/wiki-protocol.ts
---

# Interface

- `CacheIndexEntry` ← src/utils/cache-index.ts:22 [EXTRACTED]
  ```
  export interface CacheIndexEntry {
  ```
- `CacheIndex` ← src/utils/cache-index.ts:36 [EXTRACTED]
  ```
  export interface CacheIndex {
  ```
- `GcOptions` ← src/utils/cache-index.ts:42 [EXTRACTED]
  ```
  export interface GcOptions {
  ```
- `GcResult` ← src/utils/cache-index.ts:52 [EXTRACTED]
  ```
  export interface GcResult {
  ```
- `BuildIndexOptions` ← src/utils/search-index.ts:489 [EXTRACTED]
  ```
  export interface BuildIndexOptions {
  ```
- `SearchResult` ← src/utils/search-index.ts:603 [EXTRACTED]
  ```
  export interface SearchResult {
  ```
- `SkillSource` ← src/agent-skills.ts:19 [EXTRACTED]
  ```
  export type SkillSource =
  ```
- `AgentSkill` ← src/agent-skills.ts:25 [EXTRACTED]
  ```
  export interface AgentSkill {
  ```
- `AgentSkillsView` ← src/agent-skills.ts:36 [EXTRACTED]
  ```
  export interface AgentSkillsView {
  ```
- `ClassifyContext` ← src/agent-skills.ts:41 [EXTRACTED]
  ```
  export interface ClassifyContext {
  ```
- `AggregateOptions` ← src/aggregate.ts:12 [EXTRACTED]
  ```
  export interface AggregateOptions {
  ```
- `HookInput` ← src/auto-recall.ts:418 [EXTRACTED]
  ```
  export interface HookInput {
  ```
- `BuiltinHookOverride` ← src/builtin-hooks.ts:70 [EXTRACTED]
  ```
  export interface BuiltinHookOverride {
  ```
- `CacheCmdOptions` ← src/cache-cmd.ts:9 [EXTRACTED]
  ```
  export interface CacheCmdOptions extends GlobalOptions {
  ```
- `CloneOpts` ← src/clone.ts:11 [EXTRACTED]
  ```
  export interface CloneOpts {
  ```
- `CloneResult` ← src/clone.ts:22 [EXTRACTED]
  ```
  export interface CloneResult {
  ```
- `CodeKnowledgeResult` ← src/code-knowledge-recall.ts:13 [EXTRACTED]
  ```
  export interface CodeKnowledgeResult {
  ```
- `QueryCodeKnowledgeOptions` ← src/code-knowledge-recall.ts:254 [EXTRACTED]
  ```
  export interface QueryCodeKnowledgeOptions {
  ```
- `CodebaseCmdOptions` ← src/codebase-cmd.ts:15 [EXTRACTED]
  ```
  export interface CodebaseCmdOptions extends GlobalOptions {
  ```
- `ExtractCodebaseOptions` ← src/codebase-extract.ts:31 [EXTRACTED]
  ```
  export interface ExtractCodebaseOptions {
  ```
- `Severity` ← src/codebase-lint.ts:15 [EXTRACTED]
  ```
  export type Severity = 'high' | 'medium' | 'low' | 'info';
  ```
- `LintCategory` ← src/codebase-lint.ts:17 [EXTRACTED]
  ```
  export type LintCategory =
  ```
- `LintIssue` ← src/codebase-lint.ts:31 [EXTRACTED]
  ```
  export interface LintIssue {
  ```
- `LintReport` ← src/codebase-lint.ts:40 [EXTRACTED]
  ```
  export interface LintReport {
  ```
- `LintOptions` ← src/codebase-lint.ts:57 [EXTRACTED]
  ```
  export interface LintOptions {
  ```
- `FixOptions` ← src/codebase-lint.ts:65 [EXTRACTED]
  ```
  export interface FixOptions {
  ```
- `FixResult` ← src/codebase-lint.ts:71 [EXTRACTED]
  ```
  export interface FixResult {
  ```
- `UpgradeCodebaseWikiOptions` ← src/codebase-upgrade-wiki.ts:11 [EXTRACTED]
  ```
  export interface UpgradeCodebaseWikiOptions {
  ```
- `WikiLintSeverity` ← src/codebase-wiki-lint.ts:9 [EXTRACTED]
  ```
  export type WikiLintSeverity = 'high' | 'medium' | 'low' | 'info';
  ```
- `WikiLintIssue` ← src/codebase-wiki-lint.ts:11 [EXTRACTED]
  ```
  export interface WikiLintIssue {
  ```
- `WikiLintReport` ← src/codebase-wiki-lint.ts:18 [EXTRACTED]
  ```
  export interface WikiLintReport {
  ```
- `DeepEnrichOptions` ← src/deep-enrich.ts:8 [EXTRACTED]
  ```
  export interface DeepEnrichOptions {
  ```
- `InterventionSummary` ← src/digest.ts:243 [EXTRACTED]
  ```
  export interface InterventionSummary {
  ```
- `DriftCmdOptions` ← src/drift-cmd.ts:29 [EXTRACTED]
  ```
  export interface DriftCmdOptions extends GlobalOptions {
  ```
- `EnrichContext` ← src/enrich-with-ai.ts:9 [EXTRACTED]
  ```
  export interface EnrichContext {
  ```
- `EnrichResult` ← src/enrich-with-ai.ts:16 [EXTRACTED]
  ```
  export interface EnrichResult {
  ```
- `HookHandler` ← src/hook-dispatch.ts:16 [EXTRACTED]
  ```
  export interface HookHandler {
  ```
- `HandlerRegistration` ← src/hook-dispatch.ts:21 [EXTRACTED]
  ```
  export interface HandlerRegistration {
  ```
- `DispatchError` ← src/hook-dispatch.ts:29 [EXTRACTED]
  ```
  export interface DispatchError {
  ```
- `DispatchResult` ← src/hook-dispatch.ts:34 [EXTRACTED]
  ```
  export interface DispatchResult {
  ```
- `DispatcherConfig` ← src/hook-dispatch.ts:41 [EXTRACTED]
  ```
  export interface DispatcherConfig {
  ```
- `Dispatcher` ← src/hook-dispatch.ts:45 [EXTRACTED]
  ```
  export interface Dispatcher {
  ```
- `HookStatus` ← src/hooks.ts:81 [EXTRACTED]
  ```
  export type HookStatus = 'installed' | 'missing';
  ```
- `ReconcileHooksOptions` ← src/hooks.ts:116 [EXTRACTED]
  ```
  export interface ReconcileHooksOptions {
  ```
- `ManagedHookRecord` ← src/hooks.ts:131 [EXTRACTED]
  ```
  export interface ManagedHookRecord {
  ```
- `ManagedHooksManifest` ← src/hooks.ts:139 [EXTRACTED]
  ```
  export type ManagedHooksManifest = Record<string, ManagedHookRecord[]>;
  ```
- `ImportFromOrgOptions` ← src/import-org.ts:45 [EXTRACTED]
  ```
  export interface ImportFromOrgOptions {
  ```
- `ImportFromRepoListOptions` ← src/import-repo-list.ts:13 [EXTRACTED]
  ```
  export interface ImportFromRepoListOptions {
  ```
- `ImportFromRepoListResult` ← src/import-repo-list.ts:31 [EXTRACTED]
  ```
  export interface ImportFromRepoListResult {
  ```
- `ImportFromRepoOptions` ← src/import-repo.ts:34 [EXTRACTED]
  ```
  export interface ImportFromRepoOptions {
  ```
- `SectionKey` ← src/iwiki-dual.ts:40 [EXTRACTED]
  ```
  export type SectionKey = 'business-api' | 'external-knowledge' | 'glossary';
  ```
- `IWikiDualOptions` ← src/iwiki-dual.ts:43 [EXTRACTED]
  ```
  export interface IWikiDualOptions {
  ```
- `AgentCategory` ← src/known-agents.ts:16 [EXTRACTED]
  ```
  export type AgentCategory = 'coding' | 'lobster' | 'central';
  ```
- `KnownAgent` ← src/known-agents.ts:18 [EXTRACTED]
  ```
  export interface KnownAgent {
  ```
- `ResolvedAgent` ← src/known-agents.ts:75 [EXTRACTED]
  ```
  export interface ResolvedAgent extends KnownAgent {
  ```
- `MRSummary` ← src/mr-hint.ts:37 [EXTRACTED]
  ```
  export interface MRSummary {
  ```
- `RemoteRepo` ← src/mr-hint.ts:140 [EXTRACTED]
  ```
  export interface RemoteRepo {
  ```
- `ReviewCmdOptions` ← src/review-cmd.ts:27 [EXTRACTED]
  ```
  export interface ReviewCmdOptions extends GlobalOptions {
  ```
- `Risk` ← src/review-store.ts:17 [EXTRACTED]
  ```
  export type Risk = 'high' | 'medium' | 'low';
  ```
- `PendingReviewItem` ← src/review-store.ts:19 [EXTRACTED]
  ```
  export interface PendingReviewItem {
  ```
- `RoleResourceType` ← src/roles.ts:8 [EXTRACTED]
  ```
  export type RoleResourceType = typeof ROLE_RESOURCE_TYPES[number];
  ```
- `TeamRole` ← src/roles.ts:32 [EXTRACTED]
  ```
  export type TeamRole = z.infer<typeof RoleSchema>;
  ```
- `RolesManifest` ← src/roles.ts:33 [EXTRACTED]
  ```
  export type RolesManifest = z.infer<typeof RolesManifestSchema>;
  ```
- `ResourceNamespaces` ← src/roles.ts:34 [EXTRACTED]
  ```
  export type ResourceNamespaces = Record<RoleResourceType, string[]>;
  ```
- `ManagedSection` ← src/section-patcher.ts:5 [EXTRACTED]
  ```
  export interface ManagedSection {
  ```
- `SkillCommandType` ← src/skill-command.ts:22 [EXTRACTED]
  ```
  export type SkillCommandType = 'install_skill' | 'uninstall_skill' | 'update_skill';
  ```
- `SkillCommand` ← src/skill-command.ts:25 [EXTRACTED]
  ```
  export interface SkillCommand {
  ```
- `RepoFile` ← src/source-http.ts:23 [EXTRACTED]
  ```
  export interface RepoFile {
  ```
- `RepoSnapshot` ← src/source-http.ts:28 [EXTRACTED]
  ```
  export interface RepoSnapshot {
  ```
- `EndpointMap` ← src/status-report.ts:38 [EXTRACTED]
  ```
  export interface EndpointMap {
  ```
- `ReportedSkill` ← src/status-report.ts:99 [EXTRACTED]
  ```
  export interface ReportedSkill {
  ```
- `StatusReportOptions` ← src/status-report.ts:206 [EXTRACTED]
  ```
  export interface StatusReportOptions {
  ```
- `ListOptions` ← src/status.ts:22 [EXTRACTED]
  ```
  export interface ListOptions extends GlobalOptions {
  ```
- `Scope` ← src/types.ts:20 [EXTRACTED]
  ```
  export type Scope = z.infer<typeof ScopeEnum>;
  ```
- `SourceConfig` ← src/types.ts:85 [EXTRACTED]
  ```
  export type SourceConfig = z.infer<typeof SourceConfigSchema>;
  ```
- `SourceInstallManifest` ← src/types.ts:88 [EXTRACTED]
  ```
  export interface SourceInstallManifest {
  ```
- `TeamaiConfig` ← src/types.ts:136 [EXTRACTED]
  ```
  export type TeamaiConfig = z.infer<typeof TeamaiConfigSchema>;
  ```
- `MemberConfig` ← src/types.ts:147 [EXTRACTED]
  ```
  export type MemberConfig = z.infer<typeof MemberConfigSchema>;
  ```
- `LocalConfig` ← src/types.ts:172 [EXTRACTED]
  ```
  export type LocalConfig = z.infer<typeof LocalConfigSchema>;
  ```
- `LocalConfigInput` ← src/types.ts:173 [EXTRACTED]
  ```
  export type LocalConfigInput = z.input<typeof LocalConfigSchema>;
  ```
- `State` ← src/types.ts:189 [EXTRACTED]
  ```
  export type State = z.infer<typeof StateSchema>;
  ```
- `TagsConfig` ← src/types.ts:204 [EXTRACTED]
  ```
  export interface TagsConfig {
  ```
- `ResourceType` ← src/types.ts:213 [EXTRACTED]
  ```
  export type ResourceType = 'skills' | 'rules' | 'docs' | 'env' | 'wiki' | 'agents' | 'hooks';
  ```
- `ResourceItemStatus` ← src/types.ts:215 [EXTRACTED]
  ```
  export type ResourceItemStatus = 'new' | 'modified';
  ```
- `ResourceItem` ← src/types.ts:217 [EXTRACTED]
  ```
  export interface ResourceItem {
  ```
- `ResourceDiff` ← src/types.ts:226 [EXTRACTED]
  ```
  export interface ResourceDiff {
  ```
- `HookDef` ← src/types.ts:242 [EXTRACTED]
  ```
  export interface HookDef {
  ```
- `GlobalOptions` ← src/types.ts:263 [EXTRACTED]
  ```
  export interface GlobalOptions {
  ```
- `UsageEvent` ← src/types.ts:323 [EXTRACTED]
  ```
  export interface UsageEvent {
  ```
- `UserStats` ← src/types.ts:337 [EXTRACTED]
  ```
  export interface UserStats {
  ```
- `UserInterventionStats` ← src/types.ts:349 [EXTRACTED]
  ```
  export interface UserInterventionStats {
  ```
- `SessionRecord` ← src/types.ts:362 [EXTRACTED]
  ```
  export interface SessionRecord {
  ```
- `DashboardSessionStatus` ← src/types.ts:389 [EXTRACTED]
  ```
  export type DashboardSessionStatus = 'running' | 'waiting_for_input' | 'error' | 'idle' | 'stopped';
  ```
- `DashboardEventType` ← src/types.ts:391 [EXTRACTED]
  ```
  export type DashboardEventType = 'session_start' | 'tool_use' | 'prompt_submit' | 'stop' | 'process_exit';
  ```
- `DashboardEvent` ← src/types.ts:393 [EXTRACTED]
  ```
  export interface DashboardEvent {
  ```
- `DashboardSession` ← src/types.ts:426 [EXTRACTED]
  ```
  export interface DashboardSession {
  ```
- `ContributeState` ← src/types.ts:515 [EXTRACTED]
  ```
  export interface ContributeState {
  ```
- `LearningDocMeta` ← src/types.ts:581 [EXTRACTED]
  ```
  export interface LearningDocMeta {
  ```
- `KnowledgeType` ← src/types.ts:589 [EXTRACTED]
  ```
  export type KnowledgeType = 'learnings' | 'docs' | 'rules' | 'skills';
  ```
- `KnowledgeDomain` ← src/types.ts:600 [EXTRACTED]
  ```
  export type KnowledgeDomain = 'technical' | 'ops' | 'support' | 'neutral';
  ```
- `SearchIndexEntry` ← src/types.ts:603 [EXTRACTED]
  ```
  export interface SearchIndexEntry {
  ```
- `SearchIndex` ← src/types.ts:632 [EXTRACTED]
  ```
  export interface SearchIndex {
  ```
- `UserVotes` ← src/types.ts:648 [EXTRACTED]
  ```
  export interface UserVotes {
  ```
- `CultureFrontmatter` ← src/types.ts:671 [EXTRACTED]
  ```
  export type CultureFrontmatter = z.infer<typeof CultureFrontmatterSchema>;
  ```
- `MRData` ← src/types.ts:755 [EXTRACTED]
  ```
  export interface MRData {
  ```
- `ClassifiedItem` ← src/types.ts:775 [EXTRACTED]
  ```
  export interface ClassifiedItem {
  ```
- `LearningDraft` ← src/types.ts:797 [EXTRACTED]
  ```
  export interface LearningDraft {
  ```
- `CodebaseSuggestion` ← src/types.ts:809 [EXTRACTED]
  ```
  export interface CodebaseSuggestion {
  ```
- `ImportSessionItem` ← src/types.ts:847 [EXTRACTED]
  ```
  export interface ImportSessionItem {
  ```
- `ImportSession` ← src/types.ts:865 [EXTRACTED]
  ```
  export interface ImportSession {
  ```
- `UpdatePolicy` ← src/update-policy.ts:3 [EXTRACTED]
  ```
  export type UpdatePolicy = 'auto' | 'prompt' | 'skip';
  ```
- `CheckResult` ← src/update.ts:146 [EXTRACTED]
  ```
  export interface CheckResult {
  ```
- `UpdateOptions` ← src/update.ts:270 [EXTRACTED]
  ```
  export interface UpdateOptions {
  ```
- `CiExtractMrOptions` ← src/ci/extract-mr.ts:26 [EXTRACTED]
  ```
  export interface CiExtractMrOptions {
  ```
- `CommentResult` ← src/ci/mr-comment.ts:20 [EXTRACTED]
  ```
  export interface CommentResult {
  ```
- `RejectionResult` ← src/ci/read-rejections.ts:17 [EXTRACTED]
  ```
  export interface RejectionResult {
  ```
- `RecommendResult` ← src/domains/recommend.ts:6 [EXTRACTED]
  ```
  export interface RecommendResult {
  ```
- `ReviewResult` ← src/domains/review.ts:6 [EXTRACTED]
  ```
  export interface ReviewResult {
  ```
- `RepoEntry` ← src/domains/schema.ts:28 [EXTRACTED]
  ```
  export type RepoEntry = z.infer<typeof RepoEntrySchema>;
  ```
- `DomainEntry` ← src/domains/schema.ts:29 [EXTRACTED]
  ```
  export type DomainEntry = z.infer<typeof DomainEntrySchema>;
  ```
- `DomainsFile` ← src/domains/schema.ts:30 [EXTRACTED]
  ```
  export type DomainsFile = z.infer<typeof DomainsFileSchema>;
  ```
- `HistoryEvent` ← src/domains/schema.ts:39 [EXTRACTED]
  ```
  export type HistoryEvent = z.infer<typeof HistoryEventSchema>;
  ```
- `RepoMeta` ← src/domains/schema.ts:44 [EXTRACTED]
  ```
  export interface RepoMeta {
  ```
- `RepoInfo` ← src/providers/types.ts:17 [EXTRACTED]
  ```
  export interface RepoInfo {
  ```
- `PrCreateOptions` ← src/providers/types.ts:25 [EXTRACTED]
  ```
  export interface PrCreateOptions {
  ```
- `OrgRepoInfo` ← src/providers/types.ts:45 [EXTRACTED]
  ```
  export interface OrgRepoInfo {
  ```
- `GitProvider` ← src/providers/types.ts:62 [EXTRACTED]
  ```
  export interface GitProvider {
  ```
- `RepoListEntry` ← src/repo-list/schema.ts:31 [EXTRACTED]
  ```
  export type RepoListEntry = z.infer<typeof RepoListEntrySchema>;
  ```
- `RepoListOrgEntry` ← src/repo-list/schema.ts:32 [EXTRACTED]
  ```
  export type RepoListOrgEntry = z.infer<typeof RepoListOrgEntrySchema>;
  ```
- `RepoListItem` ← src/repo-list/schema.ts:33 [EXTRACTED]
  ```
  export type RepoListItem = z.infer<typeof RepoListItemSchema>;
  ```
- `RepoListFile` ← src/repo-list/schema.ts:34 [EXTRACTED]
  ```
  export type RepoListFile = z.infer<typeof RepoListFileSchema>;
  ```
- `ToolName` ← src/resources/agent-format.ts:8 [EXTRACTED]
  ```
  export type ToolName = 'claude' | 'claude-internal' | 'tclaude' | 'codebuddy' | 'codex' | 'codex-internal' | 'tcodex' | 'cursor';
  ```
- `AgentSpec` ← src/resources/agent-format.ts:28 [EXTRACTED]
  ```
  export interface AgentSpec {
  ```
- `ParseResult` ← src/resources/agent-format.ts:66 [EXTRACTED]
  ```
  export type ParseResult =
  ```
- `RenderResult` ← src/resources/agent-format.ts:129 [EXTRACTED]
  ```
  export interface RenderResult {
  ```
- `ReverseResult` ← src/resources/agent-format.ts:247 [EXTRACTED]
  ```
  export type ReverseResult =
  ```
- `MergeConflict` ← src/resources/agent-format.ts:397 [EXTRACTED]
  ```
  export interface MergeConflict {
  ```
- `MergeResult` ← src/resources/agent-format.ts:403 [EXTRACTED]
  ```
  export type MergeResult =
  ```
- `AgentResourceItem` ← src/resources/agents.ts:25 [EXTRACTED]
  ```
  export interface AgentResourceItem extends ResourceItem {
  ```
- `EnvVariable` ← src/resources/env.ts:22 [EXTRACTED]
  ```
  export type EnvVariable = z.infer<typeof EnvVariableSchema>;
  ```
- `EnvYaml` ← src/resources/env.ts:23 [EXTRACTED]
  ```
  export type EnvYaml = z.infer<typeof EnvYamlSchema>;
  ```
- `TeamHook` ← src/resources/hooks.ts:45 [EXTRACTED]
  ```
  export type TeamHook = z.infer<typeof TeamHookSchema>;
  ```
- `HooksYaml` ← src/resources/hooks.ts:46 [EXTRACTED]
  ```
  export type HooksYaml = z.infer<typeof HooksYamlSchema>;
  ```
- `BuiltinOverride` ← src/resources/hooks.ts:47 [EXTRACTED]
  ```
  export type BuiltinOverride = z.infer<typeof BuiltinOverrideSchema>;
  ```
- `IWikiPage` ← src/utils/iwiki-client.ts:31 [EXTRACTED]
  ```
  export interface IWikiPage {
  ```
- `IWikiDocument` ← src/utils/iwiki-client.ts:45 [EXTRACTED]
  ```
  export interface IWikiDocument {
  ```
- `DeriveSessionIdOptions` ← src/utils/session-id.ts:9 [EXTRACTED]
  ```
  export interface DeriveSessionIdOptions {
  ```
- `SourceMark` ← src/utils/source-conflict.ts:17 [EXTRACTED]
  ```
  export interface SourceMark {
  ```
- `TeamCodebasePaths` ← src/utils/team-codebase-paths.ts:8 [EXTRACTED]
  ```
  export interface TeamCodebasePaths {
  ```
- `CallChainLayer` ← src/wiki-engine/call-chain-tracer.ts:4 [EXTRACTED]
  ```
  export type CallChainLayer = "entry" | "orchestration" | "service" | "data";
  ```
- `CallChainStep` ← src/wiki-engine/call-chain-tracer.ts:6 [EXTRACTED]
  ```
  export interface CallChainStep {
  ```
- `CallChain` ← src/wiki-engine/call-chain-tracer.ts:14 [EXTRACTED]
  ```
  export interface CallChain {
  ```
- `DocGraphExtraction` ← src/wiki-engine/doc-graph-extractor.ts:17 [EXTRACTED]
  ```
  export interface DocGraphExtraction {
  ```
- `ExtractDocStructureOptions` ← src/wiki-engine/doc-graph-extractor.ts:22 [EXTRACTED]
  ```
  export interface ExtractDocStructureOptions {
  ```
- `InterfaceType` ← src/wiki-engine/interface-scanner.ts:6 [EXTRACTED]
  ```
  export type InterfaceType = "HTTP" | "MQ" | "RPC" | "NONE";
  ```
- `InterfaceInventoryEntry` ← src/wiki-engine/interface-scanner.ts:8 [EXTRACTED]
  ```
  export interface InterfaceInventoryEntry {
  ```
- `InterfaceInventory` ← src/wiki-engine/interface-scanner.ts:16 [EXTRACTED]
  ```
  export interface InterfaceInventory {
  ```
- `ReconcileOptions` ← src/wiki-engine/knowledge-reconciler.ts:24 [EXTRACTED]
  ```
  export interface ReconcileOptions {
  ```
- `ReconcileGraphEdge` ← src/wiki-engine/knowledge-reconciler.ts:31 [EXTRACTED]
  ```
  export interface ReconcileGraphEdge {
  ```
- `ReconcileGap` ← src/wiki-engine/knowledge-reconciler.ts:40 [EXTRACTED]
  ```
  export interface ReconcileGap {
  ```
- `ReconcileConflict` ← src/wiki-engine/knowledge-reconciler.ts:46 [EXTRACTED]
  ```
  export interface ReconcileConflict {
  ```
- `ReconcileResult` ← src/wiki-engine/knowledge-reconciler.ts:53 [EXTRACTED]
  ```
  export interface ReconcileResult {
  ```
- `CompiledComponent` ← src/wiki-engine/manifest-compiler.ts:10 [EXTRACTED]
  ```
  export interface CompiledComponent {
  ```
- `CompiledManifest` ← src/wiki-engine/manifest-compiler.ts:19 [EXTRACTED]
  ```
  export interface CompiledManifest {
  ```
- `ManifestConfidence` ← src/wiki-engine/manifest-schema.ts:24 [EXTRACTED]
  ```
  export type ManifestConfidence = "EXTRACTED" | "INFERRED" | "AMBIGUOUS";
  ```
- `ManifestEdgeSource` ← src/wiki-engine/manifest-schema.ts:27 [EXTRACTED]
  ```
  export type ManifestEdgeSource =
  ```
- `CodebaseOutputManifestV1` ← src/wiki-engine/manifest-schema.ts:56 [EXTRACTED]
  ```
  export interface CodebaseOutputManifestV1 {
  ```
- `ManifestComponentV2` ← src/wiki-engine/manifest-schema.ts:65 [EXTRACTED]
  ```
  export interface ManifestComponentV2 extends ManifestComponentBase {
  ```
- `ManifestEdgeV2` ← src/wiki-engine/manifest-schema.ts:70 [EXTRACTED]
  ```
  export interface ManifestEdgeV2 extends ManifestEdgeBase {
  ```
- `CodebaseOutputManifestV2` ← src/wiki-engine/manifest-schema.ts:77 [EXTRACTED]
  ```
  export interface CodebaseOutputManifestV2 {
  ```
- `CodebaseOutputManifest` ← src/wiki-engine/manifest-schema.ts:86 [EXTRACTED]
  ```
  export type CodebaseOutputManifest = CodebaseOutputManifestV1 | CodebaseOutputManifestV2;
  ```
- `ConfidenceFactor` ← src/wiki-engine/reconciler-v2-types.ts:5 [EXTRACTED]
  ```
  export interface ConfidenceFactor {
  ```
- `NumericConfidence` ← src/wiki-engine/reconciler-v2-types.ts:11 [EXTRACTED]
  ```
  export interface NumericConfidence {
  ```
- `ApiInterfaceMatch` ← src/wiki-engine/reconciler-v2-types.ts:48 [EXTRACTED]
  ```
  export interface ApiInterfaceMatch {
  ```
- `RuleCodeMatch` ← src/wiki-engine/reconciler-v2-types.ts:58 [EXTRACTED]
  ```
  export interface RuleCodeMatch {
  ```
- `ReconcileStaleWarning` ← src/wiki-engine/reconciler-v2-types.ts:67 [EXTRACTED]
  ```
  export interface ReconcileStaleWarning {
  ```
- `ReconcileLogEntry` ← src/wiki-engine/reconciler-v2-types.ts:78 [EXTRACTED]
  ```
  export interface ReconcileLogEntry {
  ```
- `ReconcileStats` ← src/wiki-engine/reconciler-v2-types.ts:94 [EXTRACTED]
  ```
  export interface ReconcileStats {
  ```
- `ReconcileV2Extensions` ← src/wiki-engine/reconciler-v2-types.ts:109 [EXTRACTED]
  ```
  export interface ReconcileV2Extensions {
  ```
- `GhPrCreateOptions` ← src/providers/github/gh-cli.ts:318 [EXTRACTED]
  ```
  export interface GhPrCreateOptions {
  ```
- `GfMrCreateOptions` ← src/providers/tgit/gf-cli.ts:378 [EXTRACTED]
  ```
  export interface GfMrCreateOptions {
  ```
- `DomainGroup` ← src/wiki-engine/adapters/templates.ts:1 [EXTRACTED]
  ```
  export interface DomainGroup {
  ```
- `IndexStats` ← src/wiki-engine/adapters/templates.ts:47 [EXTRACTED]
  ```
  export interface IndexStats {
  ```
- `CodeCollectedFile` ← src/wiki-engine/code-knowledge/code-collector.ts:11 [EXTRACTED]
  ```
  export interface CodeCollectedFile {
  ```
- `CodeCollectionManifest` ← src/wiki-engine/code-knowledge/code-collector.ts:35 [EXTRACTED]
  ```
  export interface CodeCollectionManifest {
  ```
- `CollectCodeOptions` ← src/wiki-engine/code-knowledge/code-collector.ts:43 [EXTRACTED]
  ```
  export interface CollectCodeOptions {
  ```
- `MultiRepoCollectOptions` ← src/wiki-engine/code-knowledge/code-collector.ts:163 [EXTRACTED]
  ```
  export interface MultiRepoCollectOptions {
  ```
- `MultiRepoManifest` ← src/wiki-engine/code-knowledge/code-collector.ts:169 [EXTRACTED]
  ```
  export interface MultiRepoManifest {
  ```
- `CodeFactKind` ← src/wiki-engine/code-knowledge/code-extractors.ts:4 [EXTRACTED]
  ```
  export type CodeFactKind = "component" | "interface" | "config" | "error" | "data" | "style" | "relation";
  ```
- `CodeEvidenceType` ← src/wiki-engine/code-knowledge/code-extractors.ts:6 [EXTRACTED]
  ```
  export type CodeEvidenceType = "definition" | "implementation" | "usage" | "schema" | "config";
  ```
- `CodeFact` ← src/wiki-engine/code-knowledge/code-extractors.ts:28 [EXTRACTED]
  ```
  export interface CodeFact {
  ```
- `CodeGraphIndex` ← src/wiki-engine/code-knowledge/code-graph.ts:19 [EXTRACTED]
  ```
  export type CodeGraphIndex = GraphIndex;
  ```
- `CodeComponent` ← src/wiki-engine/code-knowledge/code-graph.ts:78 [EXTRACTED]
  ```
  export interface CodeComponent {
  ```
- `CodeIncrementalChange` ← src/wiki-engine/code-knowledge/code-incremental.ts:6 [EXTRACTED]
  ```
  export interface CodeIncrementalChange {
  ```
- `RelationType` ← src/wiki-engine/core/graph-index.schema.ts:15 [EXTRACTED]
  ```
  export type RelationType =
  ```
- `GraphNode` ← src/wiki-engine/core/graph-index.schema.ts:34 [EXTRACTED]
  ```
  export interface GraphNode {
  ```
- `GraphEdgeSource` ← src/wiki-engine/core/graph-index.schema.ts:43 [EXTRACTED]
  ```
  export type GraphEdgeSource =
  ```
- `GraphEdge` ← src/wiki-engine/core/graph-index.schema.ts:53 [EXTRACTED]
  ```
  export interface GraphEdge {
  ```
- `GraphIndex` ← src/wiki-engine/core/graph-index.schema.ts:69 [EXTRACTED]
  ```
  export interface GraphIndex {
  ```
- `GraphValidationIssue` ← src/wiki-engine/core/graph-index.schema.ts:180 [EXTRACTED]
  ```
  export interface GraphValidationIssue {
  ```
- `GraphValidationResult` ← src/wiki-engine/core/graph-index.schema.ts:185 [EXTRACTED]
  ```
  export interface GraphValidationResult {
  ```
- `GraphHealthMetrics` ← src/wiki-engine/core/graph-index.schema.ts:244 [EXTRACTED]
  ```
  export interface GraphHealthMetrics {
  ```
- `WikiCategory` ← src/wiki-engine/core/wiki-protocol.ts:3 [EXTRACTED]
  ```
  export type WikiCategory =
  ```
- `WikiConfidence` ← src/wiki-engine/core/wiki-protocol.ts:20 [EXTRACTED]
  ```
  export type WikiConfidence = "EXTRACTED" | "INFERRED" | "AMBIGUOUS";
  ```
- `WikiReviewState` ← src/wiki-engine/core/wiki-protocol.ts:21 [EXTRACTED]
  ```
  export type WikiReviewState = "draft" | "needs-review" | "accepted";
  ```
- `WikiPageStatus` ← src/wiki-engine/core/wiki-protocol.ts:22 [EXTRACTED]
  ```
  export type WikiPageStatus = "draft" | "usable" | "stale" | "deprecated";
  ```
- `WikiEvidenceType` ← src/wiki-engine/core/wiki-protocol.ts:30 [EXTRACTED]
  ```
  export type WikiEvidenceType = "definition" | "implementation" | "usage" | "schema" | "config";
  ```
- `WikiEvidence` ← src/wiki-engine/core/wiki-protocol.ts:32 [EXTRACTED]
  ```
  export interface WikiEvidence {
  ```
- `WikiPageMetadata` ← src/wiki-engine/core/wiki-protocol.ts:46 [EXTRACTED]
  ```
  export interface WikiPageMetadata {
  ```
- `WikiPageDraft` ← src/wiki-engine/core/wiki-protocol.ts:64 [EXTRACTED]
  ```
  export interface WikiPageDraft {
  ```
- `LocalAiCommandIssue` ← src/wiki-engine/core/wiki-protocol.ts:73 [EXTRACTED]
  ```
  export interface LocalAiCommandIssue {
  ```
- `LocalAiCommandResult` ← src/wiki-engine/core/wiki-protocol.ts:80 [EXTRACTED]
  ```
  export interface LocalAiCommandResult {
  ```
- `LocalCompilePhase` ← src/wiki-engine/core/wiki-protocol.ts:94 [EXTRACTED]
  ```
  export type LocalCompilePhase =
  ```
- `LocalCompileProgress` ← src/wiki-engine/core/wiki-protocol.ts:106 [EXTRACTED]
  ```
  export interface LocalCompileProgress {
  ```