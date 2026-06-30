---
title: tgit__teamai__teamai-cli component
domain: code-knowledge
source:
  - src/rebuild-wiki-index.ts
  - src/resources/index.ts
  - src/utils/cache-index.ts
  - src/utils/search-index.ts
  - src/providers/github/index.ts
  - src/providers/tgit/index.ts
  - src/wiki-engine/code-knowledge/extractors/index.ts
  - tsup.config.ts
  - src/agent-skills.ts
  - src/aggregate.ts
  - src/api-key.ts
  - src/auto-recall.ts
  - src/builtin-agents.ts
  - src/builtin-hooks.ts
  - src/builtin-rules.ts
  - src/builtin-skills.ts
  - src/cache-cmd.ts
  - src/clone.ts
  - src/code-knowledge-recall.ts
  - src/codebase-cmd.ts
  - src/codebase-extract.ts
  - src/codebase-lint.ts
  - src/codebase-upgrade-wiki.ts
  - src/codebase-wiki-lint.ts
  - src/codebase.ts
  - src/config.ts
  - src/contribute-check.ts
  - src/contribute.ts
  - src/dashboard-collector.ts
  - src/dashboard-html.ts
  - src/dashboard.ts
  - src/deep-enrich.ts
  - src/digest.ts
  - src/doctor.ts
  - src/drift-cmd.ts
  - src/enrich-with-ai.ts
  - src/env-commands.ts
  - src/graph-aggregate.ts
  - src/hook-dispatch-cli.ts
  - src/hook-dispatch.ts
  - src/hook-handlers.ts
  - src/hooks-cmd.ts
  - src/hooks.ts
  - src/import-iwiki.ts
  - src/import-local.ts
  - src/import-mr.ts
  - src/import-org.ts
  - src/import-repo-list.ts
  - src/import-repo.ts
  - src/import.ts
  - src/init.ts
  - src/iwiki-dual.ts
  - src/known-agents.ts
  - src/machine-id.ts
  - src/members.ts
  - src/mr-hint.ts
  - src/openclaw-hooks.ts
  - src/package-info.ts
  - src/pid-monitor.ts
  - src/pull.ts
  - src/push.ts
  - src/read-only.ts
  - src/recall.ts
  - src/remove.ts
  - src/review-cmd.ts
  - src/review-store.ts
  - src/roles-cmd.ts
  - src/roles.ts
  - src/section-patcher.ts
  - src/session-collector.ts
  - src/skill-cmd.ts
  - src/skill-command.ts
  - src/skill-health.ts
  - src/skill-recommend.ts
  - src/source-http.ts
  - src/source.ts
  - src/stats.ts
  - src/status-report.ts
  - src/status.ts
  - src/tags.ts
  - src/team-push.ts
  - src/todowrite-hint.ts
  - src/types.ts
  - src/uninstall.ts
  - src/update-policy.ts
  - src/update.ts
  - src/usage-tracker.ts
  - src/ci/extract-mr.ts
  - src/ci/mr-comment.ts
  - src/ci/read-rejections.ts
  - src/domains/cluster.ts
  - src/domains/recommend.ts
  - src/domains/review.ts
  - src/domains/schema.ts
  - src/domains/store.ts
  - src/providers/registry.ts
  - src/providers/types.ts
  - src/repo-list/schema.ts
  - src/repo-list/store.ts
  - src/resources/agent-format.ts
  - src/resources/agents.ts
  - src/resources/base.ts
  - src/resources/docs.ts
  - src/resources/env.ts
  - src/resources/hooks.ts
  - src/resources/marketplace.ts
  - src/resources/rules.ts
  - src/resources/skills.ts
  - src/resources/wiki.ts
  - src/utils/ai-client.ts
  - src/utils/claudemd.ts
  - src/utils/dedup.ts
  - src/utils/fs.ts
  - src/utils/git.ts
  - src/utils/hook-output.ts
  - src/utils/iwiki-client.ts
  - src/utils/logger.ts
  - src/utils/path-safety.ts
  - src/utils/pre-push-sync.ts
  - src/utils/prompt.ts
  - src/utils/repo-cache.ts
  - src/utils/session-id.ts
  - src/utils/source-conflict.ts
  - src/utils/tags.ts
  - src/utils/team-codebase-paths.ts
  - src/utils/tool-names.ts
  - src/wiki-engine/call-chain-tracer.ts
  - src/wiki-engine/code-graph-overlay.ts
  - src/wiki-engine/doc-graph-extractor.ts
  - src/wiki-engine/interface-scanner.ts
  - src/wiki-engine/knowledge-reconciler.ts
  - src/wiki-engine/manifest-compiler.ts
  - src/wiki-engine/manifest-schema.ts
  - src/wiki-engine/reconciler-v2-types.ts
  - src/providers/github/gh-cli.ts
  - src/providers/github/gh-org.ts
  - src/providers/github/mr-fetch.ts
  - src/providers/github/repo-url.ts
  - src/providers/tgit/gf-cli.ts
  - src/providers/tgit/gf-org.ts
  - src/providers/tgit/mr-fetch.ts
  - src/providers/tgit/repo-url.ts
  - src/wiki-engine/adapters/templates.ts
  - src/wiki-engine/code-knowledge/code-collector.ts
  - src/wiki-engine/code-knowledge/code-extractors.ts
  - src/wiki-engine/code-knowledge/code-graph.ts
  - src/wiki-engine/code-knowledge/code-incremental.ts
  - src/wiki-engine/core/graph-index.schema.ts
  - src/wiki-engine/core/wiki-protocol.ts
  - src/wiki-engine/code-knowledge/extractors/config.ts
  - src/wiki-engine/code-knowledge/extractors/go.ts
  - src/wiki-engine/code-knowledge/extractors/java.ts
  - src/wiki-engine/code-knowledge/extractors/python.ts
  - src/wiki-engine/code-knowledge/extractors/rust.ts
  - src/wiki-engine/code-knowledge/extractors/typescript.ts
---

# Component

- `rebuildWikiIndex` ← src/rebuild-wiki-index.ts:19 [EXTRACTED]
  ```
  export async function rebuildWikiIndex(teamwikiRoot: string): Promise<void> {
  ```
- `getHandler` ← src/resources/index.ts:21 [EXTRACTED]
  ```
  export function getHandler(type: ResourceType): ResourceHandler {
  ```
- `getAllHandlers` ← src/resources/index.ts:25 [EXTRACTED]
  ```
  export function getAllHandlers(): ResourceHandler[] {
  ```
- `getCacheRoot` ← src/utils/cache-index.ts:64 [EXTRACTED]
  ```
  export function getCacheRoot(): string {
  ```
- `loadCacheIndex` ← src/utils/cache-index.ts:93 [EXTRACTED]
  ```
  export async function loadCacheIndex(): Promise<CacheIndex> {
  ```
- `saveCacheIndex` ← src/utils/cache-index.ts:118 [EXTRACTED]
  ```
  export async function saveCacheIndex(idx: CacheIndex): Promise<void> {
  ```
- `statDirSize` ← src/utils/cache-index.ts:139 [EXTRACTED]
  ```
  export async function statDirSize(absPath: string): Promise<number> {
  ```
- `touchCacheEntry` ← src/utils/cache-index.ts:205 [EXTRACTED]
  ```
  export async function touchCacheEntry(args: {
  ```
- `gcCache` ← src/utils/cache-index.ts:255 [EXTRACTED]
  ```
  export async function gcCache(opts?: GcOptions): Promise<GcResult> {
  ```
- `getCacheStatus` ← src/utils/cache-index.ts:382 [EXTRACTED]
  ```
  export async function getCacheStatus(): Promise<{
  ```
- `inferDomain` ← src/utils/search-index.ts:155 [EXTRACTED]
  ```
  export function inferDomain(
  ```
- `tokenize` ← src/utils/search-index.ts:213 [EXTRACTED]
  ```
  export function tokenize(text: string): string[] {
  ```
- `parseLearningDoc` ← src/utils/search-index.ts:260 [EXTRACTED]
  ```
  export function parseLearningDoc(
  ```
- `titleFromFilename` ← src/utils/search-index.ts:299 [EXTRACTED]
  ```
  export function titleFromFilename(filename: string): string {
  ```
- `buildIndex` ← src/utils/search-index.ts:506 [EXTRACTED]
  ```
  export async function buildIndex(
  ```
- `isLegacyIndex` ← src/utils/search-index.ts:584 [EXTRACTED]
  ```
  export function isLegacyIndex(index: SearchIndex | null): boolean {
  ```
- `loadIndex` ← src/utils/search-index.ts:594 [EXTRACTED]
  ```
  export async function loadIndex(indexPath?: string): Promise<SearchIndex | null> {
  ```
- `search` ← src/utils/search-index.ts:621 [EXTRACTED]
  ```
  export function search(
  ```
- `GitHubProvider` ← src/providers/github/index.ts:16 [EXTRACTED]
  ```
  export class GitHubProvider implements GitProvider {
  ```
- `TGitProvider` ← src/providers/tgit/index.ts:17 [EXTRACTED]
  ```
  export class TGitProvider implements GitProvider {
  ```
- `extractForLanguage` ← src/wiki-engine/code-knowledge/extractors/index.ts:30 [EXTRACTED]
  ```
  export function extractForLanguage(language: string, files: CodeCollectedFile[]): CodeFact[] {
  ```
- `supportedLanguages` ← src/wiki-engine/code-knowledge/extractors/index.ts:41 [EXTRACTED]
  ```
  export function supportedLanguages(): string[] {
  ```
- `defineConfig` ← tsup.config.ts:3 [INFERRED]
  ```
  export default defineConfig({
  ```
- `buildClassifyContext` ← src/agent-skills.ts:52 [EXTRACTED]
  ```
  export async function buildClassifyContext(localConfig: LocalConfig): Promise<ClassifyContext> {
  ```
- `classifySkill` ← src/agent-skills.ts:110 [EXTRACTED]
  ```
  export function classifySkill(name: string, ctx: ClassifyContext): SkillSource {
  ```
- `formatSkillSource` ← src/agent-skills.ts:122 [EXTRACTED]
  ```
  export function formatSkillSource(source: SkillSource): string {
  ```
- `scanAgentSkills` ← src/agent-skills.ts:140 [EXTRACTED]
  ```
  export async function scanAgentSkills(agent: ResolvedAgent, ctx: ClassifyContext): Promise<AgentSkillsView> {
  ```
- `scanInstalledAgents` ← src/agent-skills.ts:175 [EXTRACTED]
  ```
  export async function scanInstalledAgents(
  ```
- `readSkillDescription` ← src/agent-skills.ts:194 [EXTRACTED]
  ```
  export async function readSkillDescription(skillMdPath: string): Promise<string> {
  ```
- `truncate` ← src/agent-skills.ts:215 [EXTRACTED]
  ```
  export function truncate(text: string, max: number): string {
  ```
- `regenerateAggregate` ← src/aggregate.ts:97 [EXTRACTED]
  ```
  export async function regenerateAggregate(opts: AggregateOptions): Promise<{
  ```
- `getApiKeyPath` ← src/api-key.ts:20 [EXTRACTED]
  ```
  export function getApiKeyPath(): string {
  ```
- `resolveApiKey` ← src/api-key.ts:28 [EXTRACTED]
  ```
  export function resolveApiKey(): string | null {
  ```
- `saveApiKey` ← src/api-key.ts:44 [EXTRACTED]
  ```
  export async function saveApiKey(key: string): Promise<void> {
  ```
- `isReadOnlyCommand` ← src/auto-recall.ts:50 [EXTRACTED]
  ```
  export function isReadOnlyCommand(command: string): boolean {
  ```
- `containsError` ← src/auto-recall.ts:138 [EXTRACTED]
  ```
  export function containsError(output: string): boolean {
  ```
- `extractQuery` ← src/auto-recall.ts:162 [EXTRACTED]
  ```
  export function extractQuery(output: string): string {
  ```
- `extractGrepQuery` ← src/auto-recall.ts:232 [EXTRACTED]
  ```
  export function extractGrepQuery(toolInput: Record<string, unknown>): string {
  ```
- `extractWebSearchQuery` ← src/auto-recall.ts:255 [EXTRACTED]
  ```
  export function extractWebSearchQuery(toolInput: Record<string, unknown>): string {
  ```
- `extractWebFetchQuery` ← src/auto-recall.ts:271 [EXTRACTED]
  ```
  export function extractWebFetchQuery(toolInput: Record<string, unknown>): string {
  ```
- `shouldSkipQuery` ← src/auto-recall.ts:381 [EXTRACTED]
  ```
  export function shouldSkipQuery(sessionId: string, query: string): boolean {
  ```
- `parseHookInput` ← src/auto-recall.ts:431 [EXTRACTED]
  ```
  export function parseHookInput(data: Record<string, unknown>): HookInput | null {
  ```
- `readStdin` ← src/auto-recall.ts:465 [EXTRACTED]
  ```
  export async function readStdin(): Promise<HookInput | null> {
  ```
- `autoRecallFromInput` ← src/auto-recall.ts:502 [EXTRACTED]
  ```
  export async function autoRecallFromInput(input: HookInput): Promise<string | null> {
  ```
- `autoRecall` ← src/auto-recall.ts:666 [EXTRACTED]
  ```
  export async function autoRecall(): Promise<void> {
  ```
- `readRecallQuality` ← src/auto-recall.ts:689 [EXTRACTED]
  ```
  export function readRecallQuality(sessionId: string): { topScore: number; hitCount: number; missCount: number } | null {
  ```
- `BUILTIN_AGENT_NAMES` ← src/builtin-agents.ts:30 [EXTRACTED]
  ```
  export const BUILTIN_AGENT_NAMES = new Set<string>(['teamai-recall']);
  ```
- `deployBuiltinAgents` ← src/builtin-agents.ts:55 [EXTRACTED]
  ```
  export async function deployBuiltinAgents(
  ```
- `getDispatchCommand` ← src/builtin-hooks.ts:16 [EXTRACTED]
  ```
  export function getDispatchCommand(event: string, tool: string, matcher?: string): string {
  ```
- `builtinHookDefs` ← src/builtin-hooks.ts:56 [EXTRACTED]
  ```
  export function builtinHookDefs(tool: string): HookDef[] {
  ```
- `applyBuiltinOverride` ← src/builtin-hooks.ts:82 [EXTRACTED]
  ```
  export function applyBuiltinOverride(defs: HookDef[], override?: BuiltinHookOverride): HookDef[] {
  ```
- `BUILTIN_RULE_NAMES` ← src/builtin-rules.ts:24 [EXTRACTED]
  ```
  export const BUILTIN_RULE_NAMES = new Set<string>(['teamai-recall']);
  ```
- `EXCLUDED_RULE_NAMES` ← src/builtin-rules.ts:33 [EXTRACTED]
  ```
  export const EXCLUDED_RULE_NAMES = new Set<string>([
  ```
- `deployBuiltinRules` ← src/builtin-rules.ts:45 [EXTRACTED]
  ```
  export async function deployBuiltinRules(teamConfig: TeamaiConfig, localConfig?: LocalConfig): Promise<number> {
  ```
- `BUILTIN_SKILL_NAMES` ← src/builtin-skills.ts:41 [EXTRACTED]
  ```
  export const BUILTIN_SKILL_NAMES = new Set(['teamai-share-learnings', 'teamai-wiki', 'team-wiki-codebase']);
  ```
- `deployBuiltinSkills` ← src/builtin-skills.ts:53 [EXTRACTED]
  ```
  export async function deployBuiltinSkills(teamConfig: TeamaiConfig, localConfig?: LocalConfig, options?: { skipWiki?: boolean; reportingOnly?: boolean }): Promise<number> {
  ```
- `cacheCmd` ← src/cache-cmd.ts:57 [EXTRACTED]
  ```
  export async function cacheCmd(opts: CacheCmdOptions): Promise<void> {
  ```
- `sanitizeGitUrl` ← src/clone.ts:59 [EXTRACTED]
  ```
  export function sanitizeGitUrl(msg: string): string {
  ```
- `shallowClone` ← src/clone.ts:149 [EXTRACTED]
  ```
  export async function shallowClone(
  ```
- `shallowFetch` ← src/clone.ts:257 [EXTRACTED]
  ```
  export async function shallowFetch(
  ```
- `queryCodeKnowledge` ← src/code-knowledge-recall.ts:260 [EXTRACTED]
  ```
  export async function queryCodeKnowledge(
  ```
- `codebaseCmd` ← src/codebase-cmd.ts:64 [EXTRACTED]
  ```
  export async function codebaseCmd(opts: CodebaseCmdOptions): Promise<void> {
  ```
- `extractCodebase` ← src/codebase-extract.ts:510 [EXTRACTED]
  ```
  export async function extractCodebase(opts: ExtractCodebaseOptions): Promise<void> {
  ```
- `lintTeamCodebase` ← src/codebase-lint.ts:324 [EXTRACTED]
  ```
  export async function lintTeamCodebase(opts: LintOptions): Promise<LintReport> {
  ```
- `formatLintReport` ← src/codebase-lint.ts:741 [EXTRACTED]
  ```
  export function formatLintReport(report: LintReport, opts?: { color?: boolean }): string {
  ```
- `fixTeamCodebase` ← src/codebase-lint.ts:798 [EXTRACTED]
  ```
  export async function fixTeamCodebase(opts: FixOptions): Promise<FixResult> {
  ```
- `upgradeCodebaseWiki` ← src/codebase-upgrade-wiki.ts:23 [EXTRACTED]
  ```
  export async function upgradeCodebaseWiki(opts: UpgradeCodebaseWikiOptions): Promise<void> {
  ```
- `lintTeamwiki` ← src/codebase-wiki-lint.ts:35 [EXTRACTED]
  ```
  export async function lintTeamwiki(opts: {
  ```
- `formatWikiLintReport` ← src/codebase-wiki-lint.ts:216 [EXTRACTED]
  ```
  export function formatWikiLintReport(report: WikiLintReport): string {
  ```
- `generateCodebaseMd` ← src/codebase.ts:286 [EXTRACTED]
  ```
  export async function generateCodebaseMd(opts: {
  ```
- `generateCodebaseIndex` ← src/codebase.ts:414 [EXTRACTED]
  ```
  export async function generateCodebaseIndex(codebaseMd: string): Promise<string> {
  ```
- `lintCodebaseMd` ← src/codebase.ts:472 [EXTRACTED]
  ```
  export async function lintCodebaseMd(codebaseMd: string): Promise<LintReport> {
  ```
- `applyCodebaseSuggestions` ← src/codebase.ts:514 [EXTRACTED]
  ```
  export async function applyCodebaseSuggestions(
  ```
- `loadTeamConfig` ← src/config.ts:53 [EXTRACTED]
  ```
  export async function loadTeamConfig(repoPath: string): Promise<TeamaiConfig | null> {
  ```
- `loadLocalConfig` ← src/config.ts:71 [EXTRACTED]
  ```
  export async function loadLocalConfig(): Promise<LocalConfig | null> {
  ```
- `saveLocalConfig` ← src/config.ts:88 [EXTRACTED]
  ```
  export async function saveLocalConfig(config: LocalConfig): Promise<void> {
  ```
- `loadState` ← src/config.ts:95 [EXTRACTED]
  ```
  export async function loadState(): Promise<State> {
  ```
- `saveState` ← src/config.ts:104 [EXTRACTED]
  ```
  export async function saveState(state: State): Promise<void> {
  ```
- `requireInit` ← src/config.ts:111 [EXTRACTED]
  ```
  export async function requireInit(): Promise<{ localConfig: LocalConfig; teamConfig: TeamaiConfig }> {
  ```
- `loadLocalConfigForScope` ← src/config.ts:130 [EXTRACTED]
  ```
  export async function loadLocalConfigForScope(
  ```
- `saveLocalConfigForScope` ← src/config.ts:150 [EXTRACTED]
  ```
  export async function saveLocalConfigForScope(
  ```
- `loadStateForScope` ← src/config.ts:162 [EXTRACTED]
  ```
  export async function loadStateForScope(scope: Scope, projectRoot?: string): Promise<State> {
  ```
- `saveStateForScope` ← src/config.ts:172 [EXTRACTED]
  ```
  export async function saveStateForScope(state: State, scope: Scope, projectRoot?: string): Promise<void> {
  ```
- `detectProjectConfig` ← src/config.ts:181 [EXTRACTED]
  ```
  export async function detectProjectConfig(cwd?: string): Promise<LocalConfig | null> {
  ```
- `requireInitForScope` ← src/config.ts:202 [EXTRACTED]
  ```
  export async function requireInitForScope(
  ```
- `autoDetectInit` ← src/config.ts:226 [EXTRACTED]
  ```
  export async function autoDetectInit(): Promise<{ localConfig: LocalConfig; teamConfig: TeamaiConfig }> {
  ```
- `readContributeState` ← src/contribute-check.ts:90 [EXTRACTED]
  ```
  export async function readContributeState(sessionId: string): Promise<ContributeState> {
  ```
- `writeContributeState` ← src/contribute-check.ts:113 [EXTRACTED]
  ```
  export async function writeContributeState(sessionId: string, state: ContributeState): Promise<void> {
  ```
- `cleanupStaleSessions` ← src/contribute-check.ts:136 [EXTRACTED]
  ```
  export async function cleanupStaleSessions(dir: string, currentSessionId: string): Promise<void> {
  ```
- `computeSmartScore` ← src/contribute-check.ts:171 [EXTRACTED]
  ```
  export function computeSmartScore(events: DashboardEvent[]): number {
  ```
- `hasGitCommitInSession` ← src/contribute-check.ts:247 [EXTRACTED]
  ```
  export function hasGitCommitInSession(cwd: string, sessionStartIso: string): boolean {
  ```
- `applyPhase2Adjustments` ← src/contribute-check.ts:267 [EXTRACTED]
  ```
  export function applyPhase2Adjustments(
  ```
- `contributeCheckForSession` ← src/contribute-check.ts:377 [EXTRACTED]
  ```
  export async function contributeCheckForSession(
  ```
- `contributeCheck` ← src/contribute-check.ts:490 [EXTRACTED]
  ```
  export async function contributeCheck(toolArg?: string): Promise<void> {
  ```
- `markContributed` ← src/contribute-check.ts:508 [EXTRACTED]
  ```
  export async function markContributed(sessionId: string): Promise<void> {
  ```
- `contribute` ← src/contribute.ts:54 [EXTRACTED]
  ```
  export async function contribute(
  ```
- `readLastAssistantOutput` ← src/dashboard-collector.ts:65 [EXTRACTED]
  ```
  export async function readLastAssistantOutput(transcriptPath: string): Promise<string> {
  ```
- `countInterventions` ← src/dashboard-collector.ts:119 [EXTRACTED]
  ```
  export async function countInterventions(
  ```
- `parseHookEvent` ← src/dashboard-collector.ts:212 [EXTRACTED]
  ```
  export async function parseHookEvent(
  ```
- `appendEvent` ← src/dashboard-collector.ts:299 [EXTRACTED]
  ```
  export async function appendEvent(event: DashboardEvent): Promise<void> {
  ```
- `readEvents` ← src/dashboard-collector.ts:319 [EXTRACTED]
  ```
  export async function readEvents(eventsPath?: string): Promise<DashboardEvent[]> {
  ```
- `rebuildSessions` ← src/dashboard-collector.ts:365 [EXTRACTED]
  ```
  export function rebuildSessions(events: DashboardEvent[]): DashboardSession[] {
  ```
- `aggregateSessionInterventions` ← src/dashboard-collector.ts:497 [EXTRACTED]
  ```
  export function aggregateSessionInterventions(
  ```
- `compactEvents` ← src/dashboard-collector.ts:539 [EXTRACTED]
  ```
  export async function compactEvents(eventsPath?: string): Promise<void> {
  ```
- `dashboardReport` ← src/dashboard-collector.ts:572 [EXTRACTED]
  ```
  export async function dashboardReport(toolArg?: string): Promise<void> {
  ```
- `getDashboardHtml` ← src/dashboard-html.ts:6 [EXTRACTED]
  ```
  export function getDashboardHtml(port: number): string {
  ```
- `startDashboard` ← src/dashboard.ts:36 [EXTRACTED]
  ```
  export async function startDashboard(port?: number): Promise<void> {
  ```
- `deepEnrich` ← src/deep-enrich.ts:429 [EXTRACTED]
  ```
  export async function deepEnrich(opts: DeepEnrichOptions): Promise<void> {
  ```
- `summarizeInterventions` ← src/digest.ts:259 [EXTRACTED]
  ```
  export function summarizeInterventions(teamStats: UserStats[]): InterventionSummary | null {
  ```
- `generateDigest` ← src/digest.ts:298 [EXTRACTED]
  ```
  export async function generateDigest(options: GlobalOptions): Promise<void> {
  ```
- `doctor` ← src/doctor.ts:43 [EXTRACTED]
  ```
  export async function doctor(options: GlobalOptions): Promise<void> {
  ```
- `driftCmd` ← src/drift-cmd.ts:214 [EXTRACTED]
  ```
  export async function driftCmd(opts: DriftCmdOptions): Promise<void> {
  ```
- `enrichWithAI` ← src/enrich-with-ai.ts:88 [EXTRACTED]
  ```
  export async function enrichWithAI(ctx: EnrichContext): Promise<EnrichResult | null> {
  ```
- `writeManifest` ← src/enrich-with-ai.ts:195 [EXTRACTED]
  ```
  export async function writeManifest(manifest: CodebaseOutputManifestV2, outputDir: string): Promise<string> {
  ```
- `envList` ← src/env-commands.ts:29 [EXTRACTED]
  ```
  export async function envList(options: GlobalOptions & { reveal?: boolean }): Promise<void> {
  ```
- `envAdd` ← src/env-commands.ts:66 [EXTRACTED]
  ```
  export async function envAdd(
  ```
- `envRemove` ← src/env-commands.ts:123 [EXTRACTED]
  ```
  export async function envRemove(key: string, options: GlobalOptions): Promise<void> {
  ```
- `aggregateGlobalGraph` ← src/graph-aggregate.ts:19 [EXTRACTED]
  ```
  export async function aggregateGlobalGraph(
  ```
- `hookDispatchCli` ← src/hook-dispatch-cli.ts:25 [EXTRACTED]
  ```
  export async function hookDispatchCli(event: string, tool: string, matcher: string): Promise<void> {
  ```
- `createDispatcher` ← src/hook-dispatch.ts:76 [EXTRACTED]
  ```
  export function createDispatcher(config: DispatcherConfig): Dispatcher {
  ```
- `buildHandlerRegistry` ← src/hook-handlers.ts:235 [EXTRACTED]
  ```
  export function buildHandlerRegistry(): HandlerRegistration[] {
  ```
- `hooksInject` ← src/hooks-cmd.ts:65 [EXTRACTED]
  ```
  export async function hooksInject(options: GlobalOptions): Promise<void> {
  ```
- `hooksList` ← src/hooks-cmd.ts:88 [EXTRACTED]
  ```
  export async function hooksList(_options: GlobalOptions): Promise<void> {
  ```
- `hooksRemove` ← src/hooks-cmd.ts:137 [EXTRACTED]
  ```
  export async function hooksRemove(_options: GlobalOptions): Promise<void> {
  ```
- `TEAMAI_HOOK_SUBCOMMANDS` ← src/hooks.ts:22 [EXTRACTED]
  ```
  export const TEAMAI_HOOK_SUBCOMMANDS = ['hook-dispatch'] as const;
  ```
- `TEAMAI_LEGACY_HOOK_SUBCOMMANDS` ← src/hooks.ts:25 [EXTRACTED]
  ```
  export const TEAMAI_LEGACY_HOOK_SUBCOMMANDS = ['pull', 'update', 'track', 'track-slash', 'dashboard-report', 'contribute-check', 'auto-recall', 'todowrite-hint', 'mr-hint'] as const;
  ```
- `reconcileHooks` ← src/hooks.ts:331 [EXTRACTED]
  ```
  export async function reconcileHooks(
  ```
- `injectHooks` ← src/hooks.ts:368 [EXTRACTED]
  ```
  export async function injectHooks(settingsPath: string, tool?: string): Promise<void> {
  ```
- `removeHooks` ← src/hooks.ts:373 [EXTRACTED]
  ```
  export async function removeHooks(settingsPath: string, tool?: string): Promise<void> {
  ```
- `getHookStatus` ← src/hooks.ts:382 [EXTRACTED]
  ```
  export async function getHookStatus(settingsPath: string, tool?: string): Promise<HookStatus> {
  ```
- `injectHooksToAllTools` ← src/hooks.ts:411 [EXTRACTED]
  ```
  export async function injectHooksToAllTools(toolPaths: Record<string, { settings?: string }>, baseDir?: string): Promise<void> {
  ```
- `reconcileHooksToAllTools` ← src/hooks.ts:442 [EXTRACTED]
  ```
  export async function reconcileHooksToAllTools(
  ```
- `reconcileTeamHooksForConfig` ← src/hooks.ts:470 [EXTRACTED]
  ```
  export async function reconcileTeamHooksForConfig(
  ```
- `importFromIWiki` ← src/import-iwiki.ts:119 [EXTRACTED]
  ```
  export async function importFromIWiki(opts: {
  ```
- `scanCandidates` ← src/import-local.ts:211 [EXTRACTED]
  ```
  export async function scanCandidates(opts: {
  ```
- `classifyWithAI` ← src/import-local.ts:282 [EXTRACTED]
  ```
  export async function classifyWithAI(
  ```
- `interactiveReview` ← src/import-local.ts:332 [EXTRACTED]
  ```
  export async function interactiveReview(
  ```
- `pushAccepted` ← src/import-local.ts:497 [EXTRACTED]
  ```
  export async function pushAccepted(
  ```
- `importFromMR` ← src/import-mr.ts:251 [EXTRACTED]
  ```
  export async function importFromMR(opts: {
  ```
- `importFromOrg` ← src/import-org.ts:198 [EXTRACTED]
  ```
  export async function importFromOrg(opts: ImportFromOrgOptions): Promise<void> {
  ```
- `importFromRepoList` ← src/import-repo-list.ts:66 [EXTRACTED]
  ```
  export async function importFromRepoList(
  ```
- `detectCrossRepoEdges` ← src/import-repo.ts:86 [EXTRACTED]
  ```
  export function detectCrossRepoEdges(
  ```
- `buildRepoMetaFromPath` ← src/import-repo.ts:276 [EXTRACTED]
  ```
  export async function buildRepoMetaFromPath(
  ```
- `detectDomainDrift` ← src/import-repo.ts:417 [EXTRACTED]
  ```
  export async function detectDomainDrift(args: {
  ```
- `importFromRepo` ← src/import-repo.ts:537 [EXTRACTED]
  ```
  export async function importFromRepo(opts: ImportFromRepoOptions): Promise<void> {
  ```
- `importCmd` ← src/import.ts:83 [EXTRACTED]
  ```
  export async function importCmd(opts: ImportOptions): Promise<void> {
  ```
- `validateScopeMatch` ← src/init.ts:98 [EXTRACTED]
  ```
  export function validateScopeMatch(remoteScope: Scope | undefined, localScope: Scope): void {
  ```
- `initHttp` ← src/init.ts:114 [EXTRACTED]
  ```
  export async function initHttp(
  ```
- `init` ← src/init.ts:237 [EXTRACTED]
  ```
  export async function init(options: GlobalOptions & { repo?: string; scope?: string; role?: string; force?: boolean; http?: string; token?: string }): Promise<void> {
  ```
- `importFromIWikiDual` ← src/iwiki-dual.ts:249 [EXTRACTED]
  ```
  export async function importFromIWikiDual(opts: IWikiDualOptions): Promise<{
  ```
- `getEffectiveAgents` ← src/known-agents.ts:89 [EXTRACTED]
  ```
  export function getEffectiveAgents(teamConfig: TeamaiConfig): KnownAgent[] {
  ```
- `detectInstalledAgents` ← src/known-agents.ts:122 [EXTRACTED]
  ```
  export async function detectInstalledAgents(localConfig: LocalConfig, teamConfig: TeamaiConfig): Promise<ResolvedAgent[]> {
  ```
- `getMachineId` ← src/machine-id.ts:33 [EXTRACTED]
  ```
  export function getMachineId(): string {
  ```
- `detectMachineId` ← src/machine-id.ts:40 [EXTRACTED]
  ```
  export function detectMachineId(platform: NodeJS.Platform = process.platform): string {
  ```
- `deriveLocalAgentId` ← src/machine-id.ts:98 [EXTRACTED]
  ```
  export function deriveLocalAgentId(agentType: string, machineId: string, installPath: string): string {
  ```
- `deriveInstanceId` ← src/machine-id.ts:106 [EXTRACTED]
  ```
  export function deriveInstanceId(agentType: string, localAgentId: string): string {
  ```
- `getMemberConfig` ← src/members.ts:13 [EXTRACTED]
  ```
  export async function getMemberConfig(repoPath: string, username: string): Promise<MemberConfig | null> {
  ```
- `listMembers` ← src/members.ts:25 [EXTRACTED]
  ```
  export async function listMembers(options: GlobalOptions): Promise<void> {
  ```
- `getGitRemote` ← src/mr-hint.ts:123 [EXTRACTED]
  ```
  export function getGitRemote(cwd: string): string | null {
  ```
- `parseRemoteToRepo` ← src/mr-hint.ts:157 [EXTRACTED]
  ```
  export function parseRemoteToRepo(remoteUrl: string): RemoteRepo | null {
  ```
- `buildHintMessage` ← src/mr-hint.ts:367 [EXTRACTED]
  ```
  export function buildHintMessage(mrs: MRSummary[]): string {
  ```
- `computeMrHintOutput` ← src/mr-hint.ts:409 [EXTRACTED]
  ```
  export async function computeMrHintOutput(): Promise<string | null> {
  ```
- `mrHint` ← src/mr-hint.ts:473 [EXTRACTED]
  ```
  export async function mrHint(): Promise<void> {
  ```
- `OPENCLAW_HOOK_DIR` ← src/openclaw-hooks.ts:23 [EXTRACTED]
  ```
  export const OPENCLAW_HOOK_DIR = 'teamai-status-report';
  ```
- `handler` ← src/openclaw-hooks.ts:60 [EXTRACTED]
  ```
  export default async function handler(ctx: { event?: string } = {}): Promise<void> {
  ```
- `async` ← src/openclaw-hooks.ts:60 [INFERRED]
  ```
  export default async function handler(ctx: { event?: string } = {}): Promise<void> {
  ```
- `injectOpenClawHooks` ← src/openclaw-hooks.ts:79 [EXTRACTED]
  ```
  export async function injectOpenClawHooks(hooksDir: string, tool = 'openclaw'): Promise<void> {
  ```
- `removeOpenClawHooks` ← src/openclaw-hooks.ts:88 [EXTRACTED]
  ```
  export async function removeOpenClawHooks(hooksDir: string): Promise<void> {
  ```
- `getCurrentVersion` ← src/package-info.ts:28 [EXTRACTED]
  ```
  export function getCurrentVersion(): string {
  ```
- `getCurrentPackageName` ← src/package-info.ts:43 [EXTRACTED]
  ```
  export function getCurrentPackageName(): string {
  ```
- `getParentPid` ← src/pid-monitor.ts:20 [EXTRACTED]
  ```
  export function getParentPid(pid: number): number | undefined {
  ```
- `getProcessComm` ← src/pid-monitor.ts:54 [EXTRACTED]
  ```
  export function getProcessComm(pid: number): string | undefined {
  ```
- `resolveMonitorPid` ← src/pid-monitor.ts:84 [EXTRACTED]
  ```
  export function resolveMonitorPid(hookPpid: number): number {
  ```
- `isProcessAlive` ← src/pid-monitor.ts:111 [EXTRACTED]
  ```
  export function isProcessAlive(pid: number): boolean {
  ```
- `filterRulesByKnowledgeNamespaces` ← src/pull.ts:145 [EXTRACTED]
  ```
  export function filterRulesByKnowledgeNamespaces(
  ```
- `scanRoleAwareSkills` ← src/pull.ts:159 [EXTRACTED]
  ```
  export async function scanRoleAwareSkills(localConfig: LocalConfig, namespaces: ResourceNamespaces): Promise<ResourceItem[]> {
  ```
- `cleanupInactiveNamespaceSkills` ← src/pull.ts:184 [EXTRACTED]
  ```
  export async function cleanupInactiveNamespaceSkills(
  ```
- `compileCulture` ← src/pull.ts:855 [EXTRACTED]
  ```
  export function compileCulture(raw: string): string | null {
  ```
- `compileClaudemd` ← src/pull.ts:923 [EXTRACTED]
  ```
  export function compileClaudemd(contents: string[]): string | null {
  ```
- `compileRecallRulesBlock` ← src/pull.ts:948 [EXTRACTED]
  ```
  export function compileRecallRulesBlock(): string {
  ```
- `pull` ← src/pull.ts:1068 [EXTRACTED]
  ```
  export async function pull(options: GlobalOptions): Promise<void> {
  ```
- `filterExistingTopLevelPaths` ← src/push.ts:24 [EXTRACTED]
  ```
  export async function filterExistingTopLevelPaths(
  ```
- `push` ← src/push.ts:108 [EXTRACTED]
  ```
  export async function push(options: GlobalOptions & { all?: boolean; role?: string }): Promise<void> {
  ```
- `assertNotReadOnly` ← src/read-only.ts:10 [EXTRACTED]
  ```
  export function assertNotReadOnly(localConfig: LocalConfig, op: string): void {
  ```
- `formatResults` ← src/recall.ts:51 [EXTRACTED]
  ```
  export function formatResults(results: ScopedSearchResult[]): string {
  ```
- `autoUpvote` ← src/recall.ts:94 [EXTRACTED]
  ```
  export async function autoUpvote(
  ```
- `recall` ← src/recall.ts:222 [EXTRACTED]
  ```
  export async function recall(
  ```
- `remove` ← src/remove.ts:12 [EXTRACTED]
  ```
  export async function remove(
  ```
- `reviewCmd` ← src/review-cmd.ts:166 [EXTRACTED]
  ```
  export async function reviewCmd(opts: ReviewCmdOptions): Promise<void> {
  ```
- `PENDING_REVIEW_PATH` ← src/review-store.ts:31 [EXTRACTED]
  ```
  export const PENDING_REVIEW_PATH = '.teamai/pending-review.jsonl';
  ```
- `getPendingReviewPath` ← src/review-store.ts:47 [EXTRACTED]
  ```
  export function getPendingReviewPath(cwd: string): string {
  ```
- `computeReviewId` ← src/review-store.ts:54 [EXTRACTED]
  ```
  export function computeReviewId(
  ```
- `inferRisk` ← src/review-store.ts:71 [EXTRACTED]
  ```
  export function inferRisk(target: { file: string; section?: string }): Risk {
  ```
- `loadPendingReview` ← src/review-store.ts:140 [EXTRACTED]
  ```
  export async function loadPendingReview(cwd: string): Promise<PendingReviewItem[]> {
  ```
- `savePendingReview` ← src/review-store.ts:180 [EXTRACTED]
  ```
  export async function savePendingReview(cwd: string, items: PendingReviewItem[]): Promise<void> {
  ```
- `appendPendingReview` ← src/review-store.ts:197 [EXTRACTED]
  ```
  export async function appendPendingReview(
  ```
- `removePendingReview` ← src/review-store.ts:230 [EXTRACTED]
  ```
  export async function removePendingReview(cwd: string, id: string): Promise<boolean> {
  ```
- `rolesInit` ← src/roles-cmd.ts:76 [EXTRACTED]
  ```
  export async function rolesInit(options: GlobalOptions): Promise<void> {
  ```
- `rolesList` ← src/roles-cmd.ts:187 [EXTRACTED]
  ```
  export async function rolesList(options: GlobalOptions): Promise<void> {
  ```
- `rolesSet` ← src/roles-cmd.ts:225 [EXTRACTED]
  ```
  export async function rolesSet(
  ```
- `rolesAdd` ← src/roles-cmd.ts:290 [EXTRACTED]
  ```
  export async function rolesAdd(
  ```
- `rolesRemove` ← src/roles-cmd.ts:354 [EXTRACTED]
  ```
  export async function rolesRemove(
  ```
- `rolesUpdate` ← src/roles-cmd.ts:409 [EXTRACTED]
  ```
  export async function rolesUpdate(
  ```
- `loadRolesManifest` ← src/roles.ts:78 [EXTRACTED]
  ```
  export async function loadRolesManifest(repoPath: string): Promise<RolesManifest> {
  ```
- `saveRolesManifest` ← src/roles.ts:95 [EXTRACTED]
  ```
  export async function saveRolesManifest(repoPath: string, manifest: RolesManifest): Promise<void> {
  ```
- `findRole` ← src/roles.ts:108 [EXTRACTED]
  ```
  export function findRole(manifest: RolesManifest, roleId: string): TeamRole | undefined {
  ```
- `listRoleIds` ← src/roles.ts:112 [EXTRACTED]
  ```
  export function listRoleIds(manifest: RolesManifest): string[] {
  ```
- `describeRoles` ← src/roles.ts:116 [EXTRACTED]
  ```
  export function describeRoles(roles: Array<Pick<TeamRole, 'id' | 'description'>>): string[] {
  ```
- `resolveRoleResourceNamespaces` ← src/roles.ts:130 [EXTRACTED]
  ```
  export function resolveRoleResourceNamespaces(input: {
  ```
- `hashBody` ← src/section-patcher.ts:59 [EXTRACTED]
  ```
  export function hashBody(body: string): string {
  ```
- `splitToSections` ← src/section-patcher.ts:80 [EXTRACTED]
  ```
  export function splitToSections(md: string): { prelude: string; sections: ManagedSection[] } {
  ```
- `joinSections` ← src/section-patcher.ts:144 [EXTRACTED]
  ```
  export function joinSections(prelude: string, sections: ManagedSection[]): string {
  ```
- `parseSections` ← src/section-patcher.ts:177 [EXTRACTED]
  ```
  export function parseSections(md: string): { prelude: string; sections: ManagedSection[] } {
  ```
- `patchManagedSection` ← src/section-patcher.ts:271 [EXTRACTED]
  ```
  export function patchManagedSection(
  ```
- `mergeWithAnchors` ← src/section-patcher.ts:340 [EXTRACTED]
  ```
  export function mergeWithAnchors(
  ```
- `evaluateSessionValue` ← src/session-collector.ts:43 [EXTRACTED]
  ```
  export function evaluateSessionValue(summary: string): boolean {
  ```
- `saveSession` ← src/session-collector.ts:95 [EXTRACTED]
  ```
  export async function saveSession(summary?: string): Promise<void> {
  ```
- `skillShow` ← src/skill-cmd.ts:39 [EXTRACTED]
  ```
  export async function skillShow(name: string, options: GlobalOptions): Promise<void> {
  ```
- `installSkillZip` ← src/skill-command.ts:116 [EXTRACTED]
  ```
  export async function installSkillZip(
  ```
- `executeSkillCommand` ← src/skill-command.ts:164 [EXTRACTED]
  ```
  export async function executeSkillCommand(cmd: SkillCommand, targetSkillsDir: string): Promise<void> {
  ```
- `calculateSkillHealth` ← src/skill-health.ts:21 [EXTRACTED]
  ```
  export function calculateSkillHealth(
  ```
- `scoreToStars` ← src/skill-health.ts:41 [EXTRACTED]
  ```
  export function scoreToStars(score: number): string {
  ```
- `calculateTeamHealth` ← src/skill-health.ts:49 [EXTRACTED]
  ```
  export function calculateTeamHealth(
  ```
- `getRecommendations` ← src/skill-recommend.ts:46 [EXTRACTED]
  ```
  export async function getRecommendations(
  ```
- `displayRecommendations` ← src/skill-recommend.ts:76 [EXTRACTED]
  ```
  export function displayRecommendations(
  ```
- `RepoNotAvailableError` ← src/source-http.ts:41 [EXTRACTED]
  ```
  export class RepoNotAvailableError extends Error {
  ```
- `fetchRepoSnapshot` ← src/source-http.ts:54 [EXTRACTED]
  ```
  export async function fetchRepoSnapshot(baseUrl: string, apiKey: string): Promise<RepoSnapshot> {
  ```
- `materializeHttpRepo` ← src/source-http.ts:103 [EXTRACTED]
  ```
  export async function materializeHttpRepo(
  ```
- `removeMaterializedSkill` ← src/source-http.ts:129 [EXTRACTED]
  ```
  export async function removeMaterializedSkill(localPath: string, slug: string): Promise<void> {
  ```
- `sourceAdd` ← src/source.ts:111 [EXTRACTED]
  ```
  export async function sourceAdd(repoUrl: string, options: { name?: string } & GlobalOptions): Promise<void> {
  ```
- `sourceRemove` ← src/source.ts:173 [EXTRACTED]
  ```
  export async function sourceRemove(name: string, options: GlobalOptions): Promise<void> {
  ```
- `sourceList` ← src/source.ts:217 [EXTRACTED]
  ```
  export async function sourceList(): Promise<void> {
  ```
- `sourceBrowse` ← src/source.ts:239 [EXTRACTED]
  ```
  export async function sourceBrowse(name: string, options: GlobalOptions): Promise<void> {
  ```
- `pullSources` ← src/source.ts:299 [EXTRACTED]
  ```
  export async function pullSources(localConfig: LocalConfig, options: GlobalOptions): Promise<void> {
  ```
- `getAllSourceSkillNames` ← src/source.ts:545 [EXTRACTED]
  ```
  export async function getAllSourceSkillNames(): Promise<Set<string>> {
  ```
- `aggregateUsage` ← src/stats.ts:17 [EXTRACTED]
  ```
  export function aggregateUsage(events: UsageEvent[]): SkillStats[] {
  ```
- `showStats` ← src/stats.ts:115 [EXTRACTED]
  ```
  export async function showStats(): Promise<void> {
  ```
- `resolveEndpoints` ← src/status-report.ts:56 [EXTRACTED]
  ```
  export function resolveEndpoints(): EndpointMap {
  ```
- `getReportableAgents` ← src/status-report.ts:77 [EXTRACTED]
  ```
  export function getReportableAgents(): Set<string> {
  ```
- `resolveReportEndpoint` ← src/status-report.ts:90 [EXTRACTED]
  ```
  export function resolveReportEndpoint(localConfig: LocalConfig): string | null {
  ```
- `scanReportableSkills` ← src/status-report.ts:125 [EXTRACTED]
  ```
  export async function scanReportableSkills(skillsDir: string): Promise<ReportedSkill[]> {
  ```
- `runStatusReport` ← src/status-report.ts:219 [EXTRACTED]
  ```
  export async function runStatusReport(opts: StatusReportOptions): Promise<void> {
  ```
- `status` ← src/status.ts:30 [EXTRACTED]
  ```
  export async function status(options: GlobalOptions): Promise<void> {
  ```
- `list` ← src/status.ts:140 [EXTRACTED]
  ```
  export async function list(type: string | undefined, options: ListOptions): Promise<void> {
  ```
- `tagsList` ← src/tags.ts:13 [EXTRACTED]
  ```
  export async function tagsList(options: GlobalOptions): Promise<void> {
  ```
- `tagsSubscribe` ← src/tags.ts:64 [EXTRACTED]
  ```
  export async function tagsSubscribe(tags: string[], options: GlobalOptions): Promise<void> {
  ```
- `tagsUnsubscribe` ← src/tags.ts:98 [EXTRACTED]
  ```
  export async function tagsUnsubscribe(tags: string[], options: GlobalOptions): Promise<void> {
  ```
- `tagsAdd` ← src/tags.ts:133 [EXTRACTED]
  ```
  export async function tagsAdd(
  ```
- `tagsRemove` ← src/tags.ts:172 [EXTRACTED]
  ```
  export async function tagsRemove(
  ```
- `mergeStats` ← src/team-push.ts:63 [EXTRACTED]
  ```
  export function mergeStats(
  ```
- `computeInterventionDelta` ← src/team-push.ts:132 [EXTRACTED]
  ```
  export function computeInterventionDelta(
  ```
- `mergeInterventionStats` ← src/team-push.ts:152 [EXTRACTED]
  ```
  export function mergeInterventionStats(
  ```
- `reportUsageToTeam` ← src/team-push.ts:175 [EXTRACTED]
  ```
  export async function reportUsageToTeam(
  ```
- `getTodoWriteHintCachePath` ← src/todowrite-hint.ts:39 [EXTRACTED]
  ```
  export function getTodoWriteHintCachePath(sessionId: string): string {
  ```
- `shouldSkipTodoWriteHint` ← src/todowrite-hint.ts:77 [EXTRACTED]
  ```
  export function shouldSkipTodoWriteHint(sessionId: string): boolean {
  ```
- `todoWriteHint` ← src/todowrite-hint.ts:136 [EXTRACTED]
  ```
  export async function todoWriteHint(): Promise<void> {
  ```
- `ToolPathsSchema` ← src/types.ts:6 [EXTRACTED]
  ```
  export const ToolPathsSchema = z.object({
  ```
- `ScopeEnum` ← src/types.ts:19 [EXTRACTED]
  ```
  export const ScopeEnum = z.enum(['user', 'project']);
  ```
- `SharingConfigSchema` ← src/types.ts:24 [EXTRACTED]
  ```
  export const SharingConfigSchema = z.object({
  ```
- `getHooksSharing` ← src/types.ts:48 [EXTRACTED]
  ```
  export function getHooksSharing(config: { sharing?: { hooks?: { autoApply?: boolean; requireTeamScripts?: boolean } } }): {
  ```
- `SourceConfigSchema` ← src/types.ts:78 [EXTRACTED]
  ```
  export const SourceConfigSchema = z.object({
  ```
- `SOURCE_PULL_TTL_MS` ← src/types.ts:96 [EXTRACTED]
  ```
  export const SOURCE_PULL_TTL_MS = 24 * 60 * 60 * 1000;
  ```
- `TEAMAI_SOURCES_DIR` ← src/types.ts:98 [EXTRACTED]
  ```
  export const TEAMAI_SOURCES_DIR = `${process.env.HOME}/.teamai/sources`;
  ```
- `TeamaiConfigSchema` ← src/types.ts:100 [EXTRACTED]
  ```
  export const TeamaiConfigSchema = z.object({
  ```
- `MemberConfigSchema` ← src/types.ts:140 [EXTRACTED]
  ```
  export const MemberConfigSchema = z.object({
  ```
- `LocalConfigSchema` ← src/types.ts:151 [EXTRACTED]
  ```
  export const LocalConfigSchema = z.object({
  ```
- `StateSchema` ← src/types.ts:177 [EXTRACTED]
  ```
  export const StateSchema = z.object({
  ```
- `TEAMAI_HOME` ← src/types.ts:279 [EXTRACTED]
  ```
  export const TEAMAI_HOME = `${process.env.HOME}/.teamai`;
  ```
- `TEAMAI_STATE_PATH` ← src/types.ts:281 [EXTRACTED]
  ```
  export const TEAMAI_STATE_PATH = `${TEAMAI_HOME}/state.json`;
  ```
- `TEAMAI_TOKEN_PATH` ← src/types.ts:282 [EXTRACTED]
  ```
  export const TEAMAI_TOKEN_PATH = `${TEAMAI_HOME}/token`;
  ```
- `TEAMAI_UPDATE_LOCK_PATH` ← src/types.ts:283 [EXTRACTED]
  ```
  export const TEAMAI_UPDATE_LOCK_PATH = `${TEAMAI_HOME}/.update-lock`;
  ```
- `TEAMAI_RULES_START` ← src/types.ts:287 [EXTRACTED]
  ```
  export const TEAMAI_RULES_START = '<!-- [teamai:rules:start] -->';
  ```
- `TEAMAI_RULES_END` ← src/types.ts:288 [EXTRACTED]
  ```
  export const TEAMAI_RULES_END = '<!-- [teamai:rules:end] -->';
  ```
- `TEAMAI_HOOK_DESCRIPTION_PREFIX` ← src/types.ts:290 [EXTRACTED]
  ```
  export const TEAMAI_HOOK_DESCRIPTION_PREFIX = '[teamai]';
  ```
- `TEAMAI_CUSTOM_HOOK_PREFIX` ← src/types.ts:298 [EXTRACTED]
  ```
  export const TEAMAI_CUSTOM_HOOK_PREFIX = '[teamai:hook:';
  ```
- `TEAMAI_CULTURE_START` ← src/types.ts:303 [EXTRACTED]
  ```
  export const TEAMAI_CULTURE_START = '<!-- [teamai:culture:start] -->';
  ```
- `TEAMAI_CULTURE_END` ← src/types.ts:304 [EXTRACTED]
  ```
  export const TEAMAI_CULTURE_END = '<!-- [teamai:culture:end] -->';
  ```
- `TEAMAI_CLAUDEMD_START` ← src/types.ts:306 [EXTRACTED]
  ```
  export const TEAMAI_CLAUDEMD_START = '<!-- [teamai:claudemd:start] -->';
  ```
- `TEAMAI_CLAUDEMD_END` ← src/types.ts:307 [EXTRACTED]
  ```
  export const TEAMAI_CLAUDEMD_END = '<!-- [teamai:claudemd:end] -->';
  ```
- `TEAMAI_RECALL_RULES_START` ← src/types.ts:310 [EXTRACTED]
  ```
  export const TEAMAI_RECALL_RULES_START = '<!-- [teamai:recall-rules:start] -->';
  ```
- `TEAMAI_RECALL_RULES_END` ← src/types.ts:311 [EXTRACTED]
  ```
  export const TEAMAI_RECALL_RULES_END = '<!-- [teamai:recall-rules:end] -->';
  ```
- `SKILL_NAME_REGEX` ← src/types.ts:316 [EXTRACTED]
  ```
  export const SKILL_NAME_REGEX = /^[a-zA-Z0-9_\-:.]{1,200}$/;
  ```
- `TEAMAI_USAGE_PATH` ← src/types.ts:318 [EXTRACTED]
  ```
  export const TEAMAI_USAGE_PATH = `${TEAMAI_HOME}/usage.jsonl`;
  ```
- `TEAMAI_KNOWN_SKILLS_PATH` ← src/types.ts:319 [EXTRACTED]
  ```
  export const TEAMAI_KNOWN_SKILLS_PATH = `${TEAMAI_HOME}/known-skills.json`;
  ```
- `TEAMAI_PUSHIGNORE_PATH` ← src/types.ts:320 [EXTRACTED]
  ```
  export const TEAMAI_PUSHIGNORE_PATH = `${TEAMAI_HOME}/pushignore`;
  ```
- `TEAMAI_SESSIONS_DIR` ← src/types.ts:321 [EXTRACTED]
  ```
  export const TEAMAI_SESSIONS_DIR = `${TEAMAI_HOME}/sessions`;
  ```
- `UsageEventSchema` ← src/types.ts:329 [EXTRACTED]
  ```
  export const UsageEventSchema = z.object({
  ```
- `DASHBOARD_EVENTS_DIR` ← src/types.ts:462 [EXTRACTED]
  ```
  export const DASHBOARD_EVENTS_DIR = `${TEAMAI_HOME}/dashboard`;
  ```
- `DASHBOARD_EVENTS_PATH` ← src/types.ts:463 [EXTRACTED]
  ```
  export const DASHBOARD_EVENTS_PATH = `${DASHBOARD_EVENTS_DIR}/events.jsonl`;
  ```
- `DASHBOARD_IDLE_TIMEOUT_MS` ← src/types.ts:466 [EXTRACTED]
  ```
  export const DASHBOARD_IDLE_TIMEOUT_MS = 5 * 60 * 1000;
  ```
- `DASHBOARD_STALE_TIMEOUT_MS` ← src/types.ts:468 [EXTRACTED]
  ```
  export const DASHBOARD_STALE_TIMEOUT_MS = 30 * 60 * 1000;
  ```
- `DASHBOARD_COMPACTION_THRESHOLD` ← src/types.ts:470 [EXTRACTED]
  ```
  export const DASHBOARD_COMPACTION_THRESHOLD = 5_000;
  ```
- `DASHBOARD_STOPPED_DISPLAY_MS` ← src/types.ts:472 [EXTRACTED]
  ```
  export const DASHBOARD_STOPPED_DISPLAY_MS = 30 * 1000;
  ```
- `DASHBOARD_PID_CHECK_INTERVAL_MS` ← src/types.ts:474 [EXTRACTED]
  ```
  export const DASHBOARD_PID_CHECK_INTERVAL_MS = 15_000;
  ```
- `CORRECTION_WINDOW_MS` ← src/types.ts:484 [EXTRACTED]
  ```
  export const CORRECTION_WINDOW_MS = 60 * 1000;
  ```
- `CORRECTION_KEYWORDS` ← src/types.ts:486 [EXTRACTED]
  ```
  export const CORRECTION_KEYWORDS = [
  ```
- `INTERVENTION_SCAN_MAX_BYTES` ← src/types.ts:491 [EXTRACTED]
  ```
  export const INTERVENTION_SCAN_MAX_BYTES = 50 * 1024 * 1024;
  ```
- `TRANSCRIPT_INTERRUPT_PREFIX` ← src/types.ts:493 [EXTRACTED]
  ```
  export const TRANSCRIPT_INTERRUPT_PREFIX = '[Request interrupted by user';
  ```
- `TRANSCRIPT_REJECT_MARKERS` ← src/types.ts:495 [EXTRACTED]
  ```
  export const TRANSCRIPT_REJECT_MARKERS = [
  ```
- `CONTRIBUTE_BASE_THRESHOLD` ← src/types.ts:540 [EXTRACTED]
  ```
  export const CONTRIBUTE_BASE_THRESHOLD = 15;
  ```
- `CONTRIBUTE_SMART_THRESHOLD` ← src/types.ts:543 [EXTRACTED]
  ```
  export const CONTRIBUTE_SMART_THRESHOLD = 35;
  ```
- `CONTRIBUTE_SCORE_CACHE_MS` ← src/types.ts:546 [EXTRACTED]
  ```
  export const CONTRIBUTE_SCORE_CACHE_MS = 6 * 60 * 60 * 1000;
  ```
- `CONTRIBUTE_KNOWLEDGE_GAP_BONUS` ← src/types.ts:549 [EXTRACTED]
  ```
  export const CONTRIBUTE_KNOWLEDGE_GAP_BONUS = 20;
  ```
- `CONTRIBUTE_LOW_QUALITY_BONUS` ← src/types.ts:552 [EXTRACTED]
  ```
  export const CONTRIBUTE_LOW_QUALITY_BONUS = 10;
  ```
- `CONTRIBUTE_LOW_QUALITY_THRESHOLD` ← src/types.ts:555 [EXTRACTED]
  ```
  export const CONTRIBUTE_LOW_QUALITY_THRESHOLD = 5.0;
  ```
- `CONTRIBUTE_GIT_COMMIT_DOWNWEIGHT` ← src/types.ts:558 [EXTRACTED]
  ```
  export const CONTRIBUTE_GIT_COMMIT_DOWNWEIGHT = 0;
  ```
- `CONTRIBUTE_SESSIONS_DIR` ← src/types.ts:561 [EXTRACTED]
  ```
  export const CONTRIBUTE_SESSIONS_DIR = `${TEAMAI_HOME}/sessions`;
  ```
- `SEARCH_INDEX_VERSION` ← src/types.ts:629 [EXTRACTED]
  ```
  export const SEARCH_INDEX_VERSION = 4;
  ```
- `LEARNINGS_LOCAL_DIR` ← src/types.ts:652 [EXTRACTED]
  ```
  export const LEARNINGS_LOCAL_DIR = `${TEAMAI_HOME}/learnings`;
  ```
- `SEARCH_INDEX_PATH` ← src/types.ts:653 [EXTRACTED]
  ```
  export const SEARCH_INDEX_PATH = `${TEAMAI_HOME}/search-index.json`;
  ```
- `VOTES_LOCAL_DIR` ← src/types.ts:654 [EXTRACTED]
  ```
  export const VOTES_LOCAL_DIR = `${TEAMAI_HOME}/votes`;
  ```
- `CultureCompanySchema` ← src/types.ts:656 [EXTRACTED]
  ```
  export const CultureCompanySchema = z.object({
  ```
- `CultureTeamSchema` ← src/types.ts:662 [EXTRACTED]
  ```
  export const CultureTeamSchema = z.object({
  ```
- `CultureFrontmatterSchema` ← src/types.ts:667 [EXTRACTED]
  ```
  export const CultureFrontmatterSchema = z.object({
  ```
- `resolveBaseDir` ← src/types.ts:680 [EXTRACTED]
  ```
  export function resolveBaseDir(localConfig: LocalConfig): string {
  ```
- `getTeamaiHome` ← src/types.ts:692 [EXTRACTED]
  ```
  export function getTeamaiHome(scope: Scope, projectRoot?: string): string {
  ```
- `getConfigPath` ← src/types.ts:702 [EXTRACTED]
  ```
  export function getConfigPath(scope: Scope, projectRoot?: string): string {
  ```
- `getStatePath` ← src/types.ts:709 [EXTRACTED]
  ```
  export function getStatePath(scope: Scope, projectRoot?: string): string {
  ```
- `getManagedHooksPath` ← src/types.ts:718 [EXTRACTED]
  ```
  export function getManagedHooksPath(scope: Scope, projectRoot?: string): string {
  ```
- `getPushignorePath` ← src/types.ts:725 [EXTRACTED]
  ```
  export function getPushignorePath(): string {
  ```
- `isWikiEnabled` ← src/types.ts:734 [EXTRACTED]
  ```
  export function isWikiEnabled(): boolean {
  ```
- `areTeamHooksDisabled` ← src/types.ts:744 [EXTRACTED]
  ```
  export function areTeamHooksDisabled(): boolean {
  ```
- `uninstall` ← src/uninstall.ts:426 [EXTRACTED]
  ```
  export async function uninstall(opts: UninstallOptions): Promise<void> {
  ```
- `resolveEffectiveUpdatePolicy` ← src/update-policy.ts:10 [EXTRACTED]
  ```
  export function resolveEffectiveUpdatePolicy(
  ```
- `withUpdatePolicy` ← src/update-policy.ts:27 [EXTRACTED]
  ```
  export function withUpdatePolicy(
  ```
- `withAutoUpdate` ← src/update-policy.ts:40 [EXTRACTED]
  ```
  export function withAutoUpdate(
  ```
- `resolveRegistryForPackage` ← src/update.ts:36 [EXTRACTED]
  ```
  export function resolveRegistryForPackage(pkgName: string): string {
  ```
- `fetchLatestVersion` ← src/update.ts:49 [EXTRACTED]
  ```
  export async function fetchLatestVersion(
  ```
- `compareVersions` ← src/update.ts:73 [EXTRACTED]
  ```
  export function compareVersions(a: string, b: string): number {
  ```
- `isCacheValid` ← src/update.ts:89 [EXTRACTED]
  ```
  export function isCacheValid(lastCheck: string | null, ttlMs: number = CACHE_TTL_MS): boolean {
  ```
- `acquireLock` ← src/update.ts:105 [EXTRACTED]
  ```
  export async function acquireLock(lockPath?: string): Promise<boolean> {
  ```
- `releaseLock` ← src/update.ts:135 [EXTRACTED]
  ```
  export async function releaseLock(lockPath?: string): Promise<void> {
  ```
- `checkForUpdate` ← src/update.ts:156 [EXTRACTED]
  ```
  export async function checkForUpdate(options?: { force?: boolean }): Promise<CheckResult> {
  ```
- `doUpdate` ← src/update.ts:190 [EXTRACTED]
  ```
  export async function doUpdate(): Promise<void> {
  ```
- `update` ← src/update.ts:282 [EXTRACTED]
  ```
  export async function update(options: UpdateOptions): Promise<void> {
  ```
- `extractSkillName` ← src/usage-tracker.ts:77 [EXTRACTED]
  ```
  export function extractSkillName(toolInput: string | Record<string, unknown>): string | null {
  ```
- `isValidSkillName` ← src/usage-tracker.ts:105 [EXTRACTED]
  ```
  export function isValidSkillName(name: string): boolean {
  ```
- `skillExistsOnDisk` ← src/usage-tracker.ts:131 [EXTRACTED]
  ```
  export async function skillExistsOnDisk(skillName: string): Promise<boolean> {
  ```
- `appendUsageEvent` ← src/usage-tracker.ts:154 [EXTRACTED]
  ```
  export async function appendUsageEvent(event: UsageEvent): Promise<void> {
  ```
- `readUsageEvents` ← src/usage-tracker.ts:169 [EXTRACTED]
  ```
  export async function readUsageEvents(): Promise<UsageEvent[]> {
  ```
- `truncateUsageAfterReport` ← src/usage-tracker.ts:195 [EXTRACTED]
  ```
  export async function truncateUsageAfterReport(reportedCount: number): Promise<void> {
  ```
- `updateKnownSkills` ← src/usage-tracker.ts:217 [EXTRACTED]
  ```
  export async function updateKnownSkills(skillName: string): Promise<void> {
  ```
- `readKnownSkills` ← src/usage-tracker.ts:235 [EXTRACTED]
  ```
  export async function readKnownSkills(): Promise<Set<string>> {
  ```
- `track` ← src/usage-tracker.ts:278 [EXTRACTED]
  ```
  export async function track(rawToolName: string, toolInput: string, tool?: string): Promise<void> {
  ```
- `trackFromStdin` ← src/usage-tracker.ts:319 [EXTRACTED]
  ```
  export async function trackFromStdin(toolArg?: string): Promise<void> {
  ```
- `trackSlashCommand` ← src/usage-tracker.ts:396 [EXTRACTED]
  ```
  export async function trackSlashCommand(toolArg?: string): Promise<void> {
  ```
- `ciExtractMr` ← src/ci/extract-mr.ts:198 [EXTRACTED]
  ```
  export async function ciExtractMr(opts: CiExtractMrOptions): Promise<void> {
  ```
- `parseMrUrl` ← src/ci/mr-comment.ts:37 [EXTRACTED]
  ```
  export function parseMrUrl(url: string): ParsedMrUrl {
  ```
- `formatComment` ← src/ci/mr-comment.ts:59 [EXTRACTED]
  ```
  export function formatComment(
  ```
- `postOrUpdateMrComment` ← src/ci/mr-comment.ts:302 [EXTRACTED]
  ```
  export async function postOrUpdateMrComment(
  ```
- `formatIndividualComment` ← src/ci/mr-comment.ts:349 [EXTRACTED]
  ```
  export function formatIndividualComment(
  ```
- `postIndividualComments` ← src/ci/mr-comment.ts:398 [EXTRACTED]
  ```
  export async function postIndividualComments(
  ```
- `postCodebaseGraphComment` ← src/ci/mr-comment.ts:545 [EXTRACTED]
  ```
  export async function postCodebaseGraphComment(
  ```
- `extractMarkerId` ← src/ci/read-rejections.ts:33 [EXTRACTED]
  ```
  export function extractMarkerId(body: string): string | null {
  ```
- `readRejections` ← src/ci/read-rejections.ts:179 [EXTRACTED]
  ```
  export async function readRejections(mrUrl: string): Promise<RejectionResult> {
  ```
- `shouldWrite` ← src/ci/read-rejections.ts:198 [EXTRACTED]
  ```
  export function shouldWrite(markerId: string, rejections: RejectionResult, _provider: 'github' | 'tgit'): boolean {
  ```
- `clusterRepos` ← src/domains/cluster.ts:101 [EXTRACTED]
  ```
  export async function clusterRepos(
  ```
- `recommendDomain` ← src/domains/recommend.ts:49 [EXTRACTED]
  ```
  export async function recommendDomain(
  ```
- `reviewDomains` ← src/domains/review.ts:104 [EXTRACTED]
  ```
  export async function reviewDomains(
  ```
- `RepoEntrySchema` ← src/domains/schema.ts:4 [EXTRACTED]
  ```
  export const RepoEntrySchema = z.object({
  ```
- `DomainEntrySchema` ← src/domains/schema.ts:12 [EXTRACTED]
  ```
  export const DomainEntrySchema = z.object({
  ```
- `DomainsFileSchema` ← src/domains/schema.ts:20 [EXTRACTED]
  ```
  export const DomainsFileSchema = z.object({
  ```
- `HistoryEventSchema` ← src/domains/schema.ts:33 [EXTRACTED]
  ```
  export const HistoryEventSchema = z.object({
  ```
- `loadDomains` ← src/domains/store.ts:33 [EXTRACTED]
  ```
  export async function loadDomains(cwd: string): Promise<DomainsFile> {
  ```
- `loadDomainsDraft` ← src/domains/store.ts:52 [EXTRACTED]
  ```
  export async function loadDomainsDraft(cwd: string): Promise<DomainsFile | null> {
  ```
- `saveDomains` ← src/domains/store.ts:72 [EXTRACTED]
  ```
  export async function saveDomains(cwd: string, data: DomainsFile): Promise<void> {
  ```
- `saveDomainsDraft` ← src/domains/store.ts:84 [EXTRACTED]
  ```
  export async function saveDomainsDraft(cwd: string, data: DomainsFile): Promise<void> {
  ```
- `clearDomainsDraft` ← src/domains/store.ts:95 [EXTRACTED]
  ```
  export async function clearDomainsDraft(cwd: string): Promise<void> {
  ```
- `appendHistory` ← src/domains/store.ts:109 [EXTRACTED]
  ```
  export async function appendHistory(cwd: string, event: HistoryEvent): Promise<void> {
  ```
- `getDefaultProvider` ← src/providers/registry.ts:45 [EXTRACTED]
  ```
  export function getDefaultProvider(): string {
  ```
- `detectProvider` ← src/providers/registry.ts:68 [EXTRACTED]
  ```
  export function detectProvider(input: string): string {
  ```
- `getProvider` ← src/providers/registry.ts:101 [EXTRACTED]
  ```
  export function getProvider(providerName?: string): GitProvider {
  ```
- `getProviderFromUrl` ← src/providers/registry.ts:115 [EXTRACTED]
  ```
  export function getProviderFromUrl(repoUrl: string): GitProvider {
  ```
- `RepoNotFoundError` ← src/providers/types.ts:144 [EXTRACTED]
  ```
  export class RepoNotFoundError extends Error {
  ```
- `RepoListEntrySchema` ← src/repo-list/schema.ts:5 [EXTRACTED]
  ```
  export const RepoListEntrySchema = z.object({
  ```
- `RepoListOrgEntrySchema` ← src/repo-list/schema.ts:14 [EXTRACTED]
  ```
  export const RepoListOrgEntrySchema = z.object({
  ```
- `RepoListItemSchema` ← src/repo-list/schema.ts:23 [EXTRACTED]
  ```
  export const RepoListItemSchema = z.union([RepoListOrgEntrySchema, RepoListEntrySchema]);
  ```
- `RepoListFileSchema` ← src/repo-list/schema.ts:26 [EXTRACTED]
  ```
  export const RepoListFileSchema = z.object({
  ```
- `isOrgEntry` ← src/repo-list/schema.ts:42 [EXTRACTED]
  ```
  export function isOrgEntry(item: RepoListItem): item is RepoListOrgEntry {
  ```
- `loadRepoList` ← src/repo-list/store.ts:19 [EXTRACTED]
  ```
  export async function loadRepoList(filePath: string): Promise<RepoListFile> {
  ```
- `parseAgentYaml` ← src/resources/agent-format.ts:80 [EXTRACTED]
  ```
  export function parseAgentYaml(content: string, filename: string): ParseResult {
  ```
- `serializeAgentYaml` ← src/resources/agent-format.ts:122 [EXTRACTED]
  ```
  export function serializeAgentYaml(spec: AgentSpec): string {
  ```
- `renderForClaude` ← src/resources/agent-format.ts:138 [EXTRACTED]
  ```
  export function renderForClaude(spec: AgentSpec): RenderResult {
  ```
- `renderForClaudeInternal` ← src/resources/agent-format.ts:146 [EXTRACTED]
  ```
  export function renderForClaudeInternal(spec: AgentSpec): RenderResult {
  ```
- `renderForCodebuddy` ← src/resources/agent-format.ts:154 [EXTRACTED]
  ```
  export function renderForCodebuddy(spec: AgentSpec): RenderResult {
  ```
- `renderForCodex` ← src/resources/agent-format.ts:162 [EXTRACTED]
  ```
  export function renderForCodex(spec: AgentSpec): RenderResult {
  ```
- `renderForCodexInternal` ← src/resources/agent-format.ts:170 [EXTRACTED]
  ```
  export function renderForCodexInternal(spec: AgentSpec): RenderResult {
  ```
- `renderForCursor` ← src/resources/agent-format.ts:178 [EXTRACTED]
  ```
  export function renderForCursor(spec: AgentSpec): RenderResult {
  ```
- `reverseFromClaude` ← src/resources/agent-format.ts:263 [EXTRACTED]
  ```
  export function reverseFromClaude(filePath: string, content: string): ReverseResult {
  ```
- `reverseFromCodebuddy` ← src/resources/agent-format.ts:303 [EXTRACTED]
  ```
  export function reverseFromCodebuddy(filePath: string, content: string): ReverseResult {
  ```
- `reverseFromCodex` ← src/resources/agent-format.ts:322 [EXTRACTED]
  ```
  export function reverseFromCodex(filePath: string, content: string): ReverseResult {
  ```
- `reverseFromCursor` ← src/resources/agent-format.ts:358 [EXTRACTED]
  ```
  export function reverseFromCursor(filePath: string, content: string): ReverseResult {
  ```
- `mergeReverseResults` ← src/resources/agent-format.ts:426 [EXTRACTED]
  ```
  export function mergeReverseResults(
  ```
- `renderForTool` ← src/resources/agent-format.ts:492 [EXTRACTED]
  ```
  export function renderForTool(spec: AgentSpec, tool: ToolName): RenderResult {
  ```
- `AgentsHandler` ← src/resources/agents.ts:43 [EXTRACTED]
  ```
  export class AgentsHandler extends ResourceHandler {
  ```
- `ResourceHandler` ← src/resources/base.ts:11 [EXTRACTED]
  ```
  export abstract class ResourceHandler {
  ```
- `DocsHandler` ← src/resources/docs.ts:9 [EXTRACTED]
  ```
  export class DocsHandler extends ResourceHandler {
  ```
- `EnvHandler` ← src/resources/env.ts:37 [EXTRACTED]
  ```
  export class EnvHandler extends ResourceHandler {
  ```
- `HooksYamlSchema` ← src/resources/hooks.ts:40 [EXTRACTED]
  ```
  export const HooksYamlSchema = z.object({
  ```
- `teamHooksYamlPath` ← src/resources/hooks.ts:50 [EXTRACTED]
  ```
  export function teamHooksYamlPath(repoPath: string): string {
  ```
- `parseHooksYaml` ← src/resources/hooks.ts:58 [EXTRACTED]
  ```
  export async function parseHooksYaml(repoPath: string): Promise<HooksYaml | null> {
  ```
- `teamHookToDef` ← src/resources/hooks.ts:70 [EXTRACTED]
  ```
  export function teamHookToDef(h: TeamHook): HookDef {
  ```
- `parseTeamHooks` ← src/resources/hooks.ts:87 [EXTRACTED]
  ```
  export async function parseTeamHooks(repoPath: string): Promise<HookDef[]> {
  ```
- `parseTeamHooksConfig` ← src/resources/hooks.ts:97 [EXTRACTED]
  ```
  export async function parseTeamHooksConfig(
  ```
- `resolveTeamHooks` ← src/resources/hooks.ts:125 [EXTRACTED]
  ```
  export async function resolveTeamHooks(
  ```
- `HooksHandler` ← src/resources/hooks.ts:168 [EXTRACTED]
  ```
  export class HooksHandler extends ResourceHandler {
  ```
- `refreshMarketplace` ← src/resources/marketplace.ts:76 [EXTRACTED]
  ```
  export async function refreshMarketplace(repoPath: string): Promise<boolean> {
  ```
- `RulesHandler` ← src/resources/rules.ts:10 [EXTRACTED]
  ```
  export class RulesHandler extends ResourceHandler {
  ```
- `ensureSkillFrontmatter` ← src/resources/skills.ts:24 [EXTRACTED]
  ```
  export async function ensureSkillFrontmatter(skillDir: string, skillName: string): Promise<boolean> {
  ```
- `scanTeamRepoNamespaces` ← src/resources/skills.ts:95 [EXTRACTED]
  ```
  export async function scanTeamRepoNamespaces(repoPath: string): Promise<string[]> {
  ```
- `SkillsHandler` ← src/resources/skills.ts:207 [EXTRACTED]
  ```
  export class SkillsHandler extends ResourceHandler {
  ```
- `WikiHandler` ← src/resources/wiki.ts:35 [EXTRACTED]
  ```
  export class WikiHandler extends ResourceHandler {
  ```
- `callClaude` ← src/utils/ai-client.ts:128 [EXTRACTED]
  ```
  export async function callClaude(
  ```
- `callClaudeParallel` ← src/utils/ai-client.ts:184 [EXTRACTED]
  ```
  export async function callClaudeParallel<T>(
  ```
- `injectClaudeMdSection` ← src/utils/claudemd.ts:17 [EXTRACTED]
  ```
  export async function injectClaudeMdSection(
  ```
- `extractKeywords` ← src/utils/dedup.ts:26 [EXTRACTED]
  ```
  export function extractKeywords(text: string): Set<string> {
  ```
- `overlapRatio` ← src/utils/dedup.ts:54 [EXTRACTED]
  ```
  export function overlapRatio(a: Set<string>, b: Set<string>): number {
  ```
- `findSupersededLearnings` ← src/utils/dedup.ts:97 [EXTRACTED]
  ```
  export async function findSupersededLearnings(
  ```
- `expandHome` ← src/utils/fs.ts:21 [EXTRACTED]
  ```
  export function expandHome(p: string): string {
  ```
- `ensureDir` ← src/utils/fs.ts:31 [EXTRACTED]
  ```
  export async function ensureDir(dir: string): Promise<void> {
  ```
- `readFileSafe` ← src/utils/fs.ts:38 [EXTRACTED]
  ```
  export async function readFileSafe(filePath: string): Promise<string | null> {
  ```
- `writeFile` ← src/utils/fs.ts:49 [EXTRACTED]
  ```
  export async function writeFile(filePath: string, content: string): Promise<void> {
  ```
- `readJson` ← src/utils/fs.ts:58 [EXTRACTED]
  ```
  export async function readJson<T = unknown>(filePath: string): Promise<T | null> {
  ```
- `writeJson` ← src/utils/fs.ts:72 [EXTRACTED]
  ```
  export async function writeJson(filePath: string, data: unknown): Promise<void> {
  ```
- `copyDir` ← src/utils/fs.ts:81 [EXTRACTED]
  ```
  export async function copyDir(src: string, dest: string): Promise<void> {
  ```
- `copyFile` ← src/utils/fs.ts:100 [EXTRACTED]
  ```
  export async function copyFile(src: string, dest: string): Promise<void> {
  ```
- `listDirs` ← src/utils/fs.ts:109 [EXTRACTED]
  ```
  export async function listDirs(dirPath: string): Promise<string[]> {
  ```
- `listFiles` ← src/utils/fs.ts:119 [EXTRACTED]
  ```
  export async function listFiles(dirPath: string): Promise<string[]> {
  ```
- `listFilesRecursive` ← src/utils/fs.ts:129 [EXTRACTED]
  ```
  export async function listFilesRecursive(dirPath: string): Promise<string[]> {
  ```
- `pathExists` ← src/utils/fs.ts:153 [EXTRACTED]
  ```
  export async function pathExists(p: string): Promise<boolean> {
  ```
- `getFileMtime` ← src/utils/fs.ts:168 [EXTRACTED]
  ```
  export async function getFileMtime(filePath: string): Promise<number> {
  ```
- `getDirLatestMtime` ← src/utils/fs.ts:181 [EXTRACTED]
  ```
  export async function getDirLatestMtime(dirPath: string): Promise<number> {
  ```
- `fileContentEqualToBuffer` ← src/utils/fs.ts:218 [EXTRACTED]
  ```
  export async function fileContentEqualToBuffer(filePath: string, buffer: Buffer): Promise<boolean> {
  ```
- `fileContentEqual` ← src/utils/fs.ts:229 [EXTRACTED]
  ```
  export async function fileContentEqual(fileA: string, fileB: string): Promise<boolean> {
  ```
- `dirContentEqual` ← src/utils/fs.ts:243 [EXTRACTED]
  ```
  export async function dirContentEqual(dirA: string, dirB: string, ignore?: string[]): Promise<boolean> {
  ```
- `dirTeamSubsetEqual` ← src/utils/fs.ts:283 [EXTRACTED]
  ```
  export async function dirTeamSubsetEqual(
  ```
- `createGit` ← src/utils/git.ts:12 [EXTRACTED]
  ```
  export function createGit(basePath?: string): SimpleGit {
  ```
- `initRepo` ← src/utils/git.ts:23 [EXTRACTED]
  ```
  export async function initRepo(remote: string, localPath: string): Promise<void> {
  ```
- `configureGitUser` ← src/utils/git.ts:37 [EXTRACTED]
  ```
  export async function configureGitUser(
  ```
- `getHeadRev` ← src/utils/git.ts:62 [EXTRACTED]
  ```
  export async function getHeadRev(localPath: string): Promise<string> {
  ```
- `pullRepo` ← src/utils/git.ts:67 [EXTRACTED]
  ```
  export async function pullRepo(localPath: string): Promise<string> {
  ```
- `getDefaultBranch` ← src/utils/git.ts:86 [EXTRACTED]
  ```
  export async function getDefaultBranch(localPath: string): Promise<string> {
  ```
- `pushRepoDirectly` ← src/utils/git.ts:122 [EXTRACTED]
  ```
  export async function pushRepoDirectly(localPath: string, message: string, files: string[]): Promise<void> {
  ```
- `autoPushTeamRepo` ← src/utils/git.ts:149 [EXTRACTED]
  ```
  export async function autoPushTeamRepo(repoPath: string, message: string): Promise<void> {
  ```
- `pushRepoBranch` ← src/utils/git.ts:165 [EXTRACTED]
  ```
  export async function pushRepoBranch(
  ```
- `checkoutMaster` ← src/utils/git.ts:198 [EXTRACTED]
  ```
  export async function checkoutMaster(localPath: string): Promise<void> {
  ```
- `generateBranchName` ← src/utils/git.ts:207 [EXTRACTED]
  ```
  export function generateBranchName(username: string): string {
  ```
- `resetToCleanMaster` ← src/utils/git.ts:228 [EXTRACTED]
  ```
  export async function resetToCleanMaster(git: SimpleGit, localPath?: string): Promise<void> {
  ```
- `getFileContentAtRev` ← src/utils/git.ts:269 [EXTRACTED]
  ```
  export async function getFileContentAtRev(
  ```
- `getRepoStatus` ← src/utils/git.ts:283 [EXTRACTED]
  ```
  export async function getRepoStatus(localPath: string): Promise<{ ahead: number; behind: number; modified: string[] }> {
  ```
- `formatStopHookOutput` ← src/utils/hook-output.ts:17 [EXTRACTED]
  ```
  export function formatStopHookOutput(message: string, tool: string): string {
  ```
- `IWikiClient` ← src/utils/iwiki-client.ts:82 [EXTRACTED]
  ```
  export class IWikiClient {
  ```
- `MAX_LOG_BYTES` ← src/utils/logger.ts:21 [EXTRACTED]
  ```
  export const MAX_LOG_BYTES = 5 * 1024 * 1024; // 5 MB
  ```
- `_setLogFilePath` ← src/utils/logger.ts:92 [EXTRACTED]
  ```
  export function _setLogFilePath(p: string): void {
  ```
- `_resetState` ← src/utils/logger.ts:98 [EXTRACTED]
  ```
  export function _resetState(): void {
  ```
- `setVerbose` ← src/utils/logger.ts:106 [EXTRACTED]
  ```
  export function setVerbose(v: boolean): void {
  ```
- `setSilent` ← src/utils/logger.ts:110 [EXTRACTED]
  ```
  export function setSilent(s: boolean): void {
  ```
- `log` ← src/utils/logger.ts:114 [EXTRACTED]
  ```
  export const log = {
  ```
- `spinner` ← src/utils/logger.ts:142 [EXTRACTED]
  ```
  export function spinner(text: string): Ora {
  ```
- `assertSafePath` ← src/utils/path-safety.ts:15 [EXTRACTED]
  ```
  export function assertSafePath(target: string, allowedRoots: string[]): void {
  ```
- `assertWithinRoot` ← src/utils/path-safety.ts:44 [EXTRACTED]
  ```
  export function assertWithinRoot(root: string, candidate: string, message?: string): void {
  ```
- `defaultAllowedRoots` ← src/utils/path-safety.ts:80 [EXTRACTED]
  ```
  export function defaultAllowedRoots(): string[] {
  ```
- `assertSafeResourceName` ← src/utils/path-safety.ts:99 [EXTRACTED]
  ```
  export function assertSafeResourceName(name: string): void {
  ```
- `syncTeamUpdatesToLocal` ← src/utils/pre-push-sync.ts:35 [EXTRACTED]
  ```
  export async function syncTeamUpdatesToLocal(
  ```
- `closePrompt` ← src/utils/prompt.ts:31 [EXTRACTED]
  ```
  export function closePrompt(): void {
  ```
- `askQuestion` ← src/utils/prompt.ts:67 [EXTRACTED]
  ```
  export function askQuestion(prompt: string, defaultValue?: string): Promise<string> {
  ```
- `askConfirmation` ← src/utils/prompt.ts:85 [EXTRACTED]
  ```
  export function askConfirmation(
  ```
- `parseSelection` ← src/utils/prompt.ts:111 [EXTRACTED]
  ```
  export function parseSelection(input: string, maxItems: number): number[] | null {
  ```
- `askSelection` ← src/utils/prompt.ts:151 [EXTRACTED]
  ```
  export async function askSelection(
  ```
- `getRepoCacheDir` ← src/utils/repo-cache.ts:28 [EXTRACTED]
  ```
  export function getRepoCacheDir(provider: string, owner: string, repo: string): string {
  ```
- `getRepoSlug` ← src/utils/repo-cache.ts:39 [EXTRACTED]
  ```
  export function getRepoSlug(provider: string, owner: string, repo: string): string {
  ```
- `writeLastSync` ← src/utils/repo-cache.ts:50 [EXTRACTED]
  ```
  export async function writeLastSync(cacheDir: string, sha: string): Promise<void> {
  ```
- `readLastSync` ← src/utils/repo-cache.ts:61 [EXTRACTED]
  ```
  export async function readLastSync(
  ```
- `ensureCacheRoot` ← src/utils/repo-cache.ts:80 [EXTRACTED]
  ```
  export async function ensureCacheRoot(): Promise<string> {
  ```
- `deriveSessionId` ← src/utils/session-id.ts:22 [EXTRACTED]
  ```
  export function deriveSessionId(
  ```
- `recordSourceUpdate` ← src/utils/source-conflict.ts:78 [EXTRACTED]
  ```
  export async function recordSourceUpdate(
  ```
- `loadTagsConfig` ← src/utils/tags.ts:16 [EXTRACTED]
  ```
  export async function loadTagsConfig(repoPath: string): Promise<TagsConfig | null> {
  ```
- `filterByTags` ← src/utils/tags.ts:64 [EXTRACTED]
  ```
  export function filterByTags(
  ```
- `saveTagsConfig` ← src/utils/tags.ts:104 [EXTRACTED]
  ```
  export async function saveTagsConfig(repoPath: string, config: TagsConfig): Promise<void> {
  ```
- `collectTagStats` ← src/utils/tags.ts:116 [EXTRACTED]
  ```
  export function collectTagStats(
  ```
- `TEAM_CODEBASE_DIR` ← src/utils/team-codebase-paths.ts:5 [EXTRACTED]
  ```
  export const TEAM_CODEBASE_DIR = 'team-codebase';
  ```
- `getTeamCodebasePaths` ← src/utils/team-codebase-paths.ts:26 [EXTRACTED]
  ```
  export function getTeamCodebasePaths(cwd: string, output?: string): TeamCodebasePaths {
  ```
- `safeDomainSlug` ← src/utils/team-codebase-paths.ts:45 [EXTRACTED]
  ```
  export function safeDomainSlug(name: string): string {
  ```
- `normalizeToolName` ← src/utils/tool-names.ts:21 [EXTRACTED]
  ```
  export function normalizeToolName(name: string): string {
  ```
- `traceCallChains` ← src/wiki-engine/call-chain-tracer.ts:76 [EXTRACTED]
  ```
  export function traceCallChains(facts: CodeFact[], files: CodeCollectedFile[]): CallChain[] {
  ```
- `buildIndexHubOverlay` ← src/wiki-engine/code-graph-overlay.ts:9 [EXTRACTED]
  ```
  export function buildIndexHubOverlay(
  ```
- `sectionNodeSlug` ← src/wiki-engine/doc-graph-extractor.ts:31 [EXTRACTED]
  ```
  export function sectionNodeSlug(pageSlug: string, sectionSlug: string): string {
  ```
- `extractDocStructure` ← src/wiki-engine/doc-graph-extractor.ts:35 [EXTRACTED]
  ```
  export function extractDocStructure(
  ```
- `extractDocEntities` ← src/wiki-engine/doc-graph-extractor.ts:105 [EXTRACTED]
  ```
  export function extractDocEntities(
  ```
- `wikiLinkToPageSlug` ← src/wiki-engine/doc-graph-extractor.ts:184 [EXTRACTED]
  ```
  export function wikiLinkToPageSlug(link: string): string {
  ```
- `entitySlugFor` ← src/wiki-engine/doc-graph-extractor.ts:193 [EXTRACTED]
  ```
  export function entitySlugFor(kind: string, anchor: string): string {
  ```
- `scanInterfaces` ← src/wiki-engine/interface-scanner.ts:70 [EXTRACTED]
  ```
  export async function scanInterfaces(files: CodeCollectedFile[]): Promise<InterfaceInventory> {
  ```
- `scanInterfacesFromFacts` ← src/wiki-engine/interface-scanner.ts:178 [EXTRACTED]
  ```
  export async function scanInterfacesFromFacts(
  ```
- `reconcileKnowledge` ← src/wiki-engine/knowledge-reconciler.ts:189 [EXTRACTED]
  ```
  export async function reconcileKnowledge(options: ReconcileOptions): Promise<ReconcileResult> {
  ```
- `compileFromManifest` ← src/wiki-engine/manifest-compiler.ts:26 [EXTRACTED]
  ```
  export async function compileFromManifest(manifestPath: string): Promise<CompiledManifest> {
  ```
- `isManifestV2` ← src/wiki-engine/manifest-schema.ts:88 [EXTRACTED]
  ```
  export function isManifestV2(manifest: CodebaseOutputManifest): manifest is CodebaseOutputManifestV2 {
  ```
- `fromLegacyConfidence` ← src/wiki-engine/reconciler-v2-types.ts:18 [EXTRACTED]
  ```
  export function fromLegacyConfidence(confidence: WikiConfidence): NumericConfidence {
  ```
- `labelFromScore` ← src/wiki-engine/reconciler-v2-types.ts:32 [EXTRACTED]
  ```
  export function labelFromScore(score: number): WikiConfidence {
  ```
- `buildConfidence` ← src/wiki-engine/reconciler-v2-types.ts:39 [EXTRACTED]
  ```
  export function buildConfidence(factors: ConfidenceFactor[]): NumericConfidence {
  ```
- `isGhInstalled` ← src/providers/github/gh-cli.ts:32 [EXTRACTED]
  ```
  export function isGhInstalled(): boolean {
  ```
- `ghExec` ← src/providers/github/gh-cli.ts:40 [EXTRACTED]
  ```
  export function ghExec(
  ```
- `ensureGhAvailable` ← src/providers/github/gh-cli.ts:82 [EXTRACTED]
  ```
  export async function ensureGhAvailable(): Promise<void> {
  ```
- `getGitHubToken` ← src/providers/github/gh-cli.ts:108 [EXTRACTED]
  ```
  export function getGitHubToken(): string | null {
  ```
- `ghGetOAuthToken` ← src/providers/github/gh-cli.ts:118 [EXTRACTED]
  ```
  export function ghGetOAuthToken(): string | null {
  ```
- `ghIsAuthenticated` ← src/providers/github/gh-cli.ts:138 [EXTRACTED]
  ```
  export function ghIsAuthenticated(): boolean {
  ```
- `ghFetchLogin` ← src/providers/github/gh-cli.ts:153 [EXTRACTED]
  ```
  export async function ghFetchLogin(token: string): Promise<string | null> {
  ```
- `ghAuthWhoami` ← src/providers/github/gh-cli.ts:174 [EXTRACTED]
  ```
  export async function ghAuthWhoami(): Promise<string | null> {
  ```
- `ghAuthLogin` ← src/providers/github/gh-cli.ts:196 [EXTRACTED]
  ```
  export function ghAuthLogin(): void {
  ```
- `ensureGhAuthenticated` ← src/providers/github/gh-cli.ts:216 [EXTRACTED]
  ```
  export async function ensureGhAuthenticated(): Promise<string> {
  ```
- `ghRepoClone` ← src/providers/github/gh-cli.ts:245 [EXTRACTED]
  ```
  export function ghRepoClone(repo: string, localPath: string): void {
  ```
- `ghCreateRepo` ← src/providers/github/gh-cli.ts:277 [EXTRACTED]
  ```
  export async function ghCreateRepo(owner: string, repo: string): Promise<void> {
  ```
- `ghPrCreate` ← src/providers/github/gh-cli.ts:342 [EXTRACTED]
  ```
  export async function ghPrCreate(opts: GhPrCreateOptions): Promise<string> {
  ```
- `ghListOrgRepos` ← src/providers/github/gh-org.ts:119 [EXTRACTED]
  ```
  export async function ghListOrgRepos(
  ```
- `fetchGitHubPR` ← src/providers/github/mr-fetch.ts:152 [EXTRACTED]
  ```
  export async function fetchGitHubPR(url: string): Promise<MRData> {
  ```
- `parseGitHubRepoInput` ← src/providers/github/repo-url.ts:15 [EXTRACTED]
  ```
  export function parseGitHubRepoInput(input: string): RepoInfo {
  ```
- `gfExec` ← src/providers/tgit/gf-cli.ts:33 [EXTRACTED]
  ```
  export function gfExec(
  ```
- `isGfInstalled` ← src/providers/tgit/gf-cli.ts:129 [EXTRACTED]
  ```
  export function isGfInstalled(): boolean {
  ```
- `ensureGfInstalled` ← src/providers/tgit/gf-cli.ts:141 [EXTRACTED]
  ```
  export async function ensureGfInstalled(): Promise<void> {
  ```
- `gfIsAuthenticated` ← src/providers/tgit/gf-cli.ts:176 [EXTRACTED]
  ```
  export function gfIsAuthenticated(): boolean {
  ```
- `gfAuthWhoami` ← src/providers/tgit/gf-cli.ts:189 [EXTRACTED]
  ```
  export function gfAuthWhoami(): string | null {
  ```
- `gfAuthLogin` ← src/providers/tgit/gf-cli.ts:207 [EXTRACTED]
  ```
  export function gfAuthLogin(): void {
  ```
- `ensureAuthenticated` ← src/providers/tgit/gf-cli.ts:219 [EXTRACTED]
  ```
  export function ensureAuthenticated(): string {
  ```
- `gfGetOAuthToken` ← src/providers/tgit/gf-cli.ts:252 [EXTRACTED]
  ```
  export function gfGetOAuthToken(): string | null {
  ```
- `gfCreateRepo` ← src/providers/tgit/gf-cli.ts:272 [EXTRACTED]
  ```
  export async function gfCreateRepo(owner: string, repo: string): Promise<void> {
  ```
- `gfRepoClone` ← src/providers/tgit/gf-cli.ts:338 [EXTRACTED]
  ```
  export function gfRepoClone(repo: string, localPath: string): void {
  ```
- `gfMrCreate` ← src/providers/tgit/gf-cli.ts:399 [EXTRACTED]
  ```
  export function gfMrCreate(opts: GfMrCreateOptions): string {
  ```
- `gfListOrgRepos` ← src/providers/tgit/gf-org.ts:56 [EXTRACTED]
  ```
  export async function gfListOrgRepos(
  ```
- `fetchTGitMR` ← src/providers/tgit/mr-fetch.ts:100 [EXTRACTED]
  ```
  export async function fetchTGitMR(url: string): Promise<MRData> {
  ```
- `parseTGitRepoInput` ← src/providers/tgit/repo-url.ts:13 [EXTRACTED]
  ```
  export function parseTGitRepoInput(input: string): RepoInfo {
  ```
- `routerTemplate` ← src/wiki-engine/adapters/templates.ts:7 [EXTRACTED]
  ```
  export function routerTemplate(
  ```
- `indexTemplate` ← src/wiki-engine/adapters/templates.ts:55 [EXTRACTED]
  ```
  export function indexTemplate(
  ```
- `HOT_TEMPLATE` ← src/wiki-engine/adapters/templates.ts:89 [EXTRACTED]
  ```
  export const HOT_TEMPLATE = [
  ```
- `isKeyFile` ← src/wiki-engine/code-knowledge/code-collector.ts:29 [EXTRACTED]
  ```
  export function isKeyFile(relativePath: string, language: string): boolean {
  ```
- `collectCode` ← src/wiki-engine/code-knowledge/code-collector.ts:50 [EXTRACTED]
  ```
  export async function collectCode(options: CollectCodeOptions): Promise<{ manifest: CodeCollectionManifest; files: CodeCollectedFile[] }> {
  ```
- `collectMultiRepo` ← src/wiki-engine/code-knowledge/code-collector.ts:176 [EXTRACTED]
  ```
  export async function collectMultiRepo(options: MultiRepoCollectOptions): Promise<{
  ```
- `mapKindToEvidenceType` ← src/wiki-engine/code-knowledge/code-extractors.ts:11 [EXTRACTED]
  ```
  export function mapKindToEvidenceType(kind: CodeFactKind): CodeEvidenceType {
  ```
- `extractCodeFacts` ← src/wiki-engine/code-knowledge/code-extractors.ts:43 [EXTRACTED]
  ```
  export function extractCodeFacts(files: CodeCollectedFile[]): CodeFact[] {
  ```
- `writeCodeGraph` ← src/wiki-engine/code-knowledge/code-graph.ts:21 [EXTRACTED]
  ```
  export async function writeCodeGraph(wikiRoot: string, project: string, facts: CodeFact[]): Promise<{ graph: GraphIndex; path: string }> {
  ```
- `buildCodeGraph` ← src/wiki-engine/code-knowledge/code-graph.ts:32 [EXTRACTED]
  ```
  export function buildCodeGraph(facts: CodeFact[]): GraphIndex {
  ```
- `buildCodeGraphIndex` ← src/wiki-engine/code-knowledge/code-graph.ts:93 [EXTRACTED]
  ```
  export function buildCodeGraphIndex(components: Array<{
  ```
- `detectCodeIncrementalChanges` ← src/wiki-engine/code-knowledge/code-incremental.ts:13 [EXTRACTED]
  ```
  export async function detectCodeIncrementalChanges(root: string, manifestPath: string, project: string): Promise<CodeIncrementalChange> {
  ```
- `GRAPH_INDEX_SCHEMA_VERSION` ← src/wiki-engine/core/graph-index.schema.ts:13 [EXTRACTED]
  ```
  export const GRAPH_INDEX_SCHEMA_VERSION = "team-wiki.graph-index.v1" as const;
  ```
- `toPageSlug` ← src/wiki-engine/core/graph-index.schema.ts:65 [EXTRACTED]
  ```
  export function toPageSlug(relativePath: string): string {
  ```
- `createGraphIndex` ← src/wiki-engine/core/graph-index.schema.ts:79 [EXTRACTED]
  ```
  export function createGraphIndex(nodes: GraphNode[] = [], edges: GraphEdge[] = []): GraphIndex {
  ```
- `addNode` ← src/wiki-engine/core/graph-index.schema.ts:92 [EXTRACTED]
  ```
  export function addNode(graph: GraphIndex, node: GraphNode): GraphIndex {
  ```
- `addEdge` ← src/wiki-engine/core/graph-index.schema.ts:100 [EXTRACTED]
  ```
  export function addEdge(graph: GraphIndex, edge: GraphEdge): GraphIndex {
  ```
- `addEdgeWithConfidence` ← src/wiki-engine/core/graph-index.schema.ts:114 [EXTRACTED]
  ```
  export function addEdgeWithConfidence(
  ```
- `findNeighbors` ← src/wiki-engine/core/graph-index.schema.ts:126 [EXTRACTED]
  ```
  export function findNeighbors(graph: GraphIndex, slug: string): string[] {
  ```
- `findNeighborsNHop` ← src/wiki-engine/core/graph-index.schema.ts:144 [EXTRACTED]
  ```
  export function findNeighborsNHop(
  ```
- `validateGraph` ← src/wiki-engine/core/graph-index.schema.ts:197 [EXTRACTED]
  ```
  export function validateGraph(graph: GraphIndex): GraphValidationResult {
  ```
- `computeGraphHealth` ← src/wiki-engine/core/graph-index.schema.ts:267 [EXTRACTED]
  ```
  export function computeGraphHealth(graph: GraphIndex): GraphHealthMetrics {
  ```
- `loadGraphIndex` ← src/wiki-engine/core/graph-index.schema.ts:351 [EXTRACTED]
  ```
  export async function loadGraphIndex(wikiRoot: string): Promise<GraphIndex | null> {
  ```
- `saveGraphIndex` ← src/wiki-engine/core/graph-index.schema.ts:365 [EXTRACTED]
  ```
  export async function saveGraphIndex(wikiRoot: string, graph: GraphIndex): Promise<string> {
  ```
- `mergeGraphs` ← src/wiki-engine/core/graph-index.schema.ts:382 [EXTRACTED]
  ```
  export function mergeGraphs(base: GraphIndex, overlay: GraphIndex): GraphIndex {
  ```
- `safeIgnore` ← src/wiki-engine/core/wiki-protocol.ts:153 [EXTRACTED]
  ```
  export function safeIgnore(filePath: string): boolean {
  ```
- `slugifyWiki` ← src/wiki-engine/core/wiki-protocol.ts:166 [EXTRACTED]
  ```
  export function slugifyWiki(value: string): string {
  ```
- `wikiPagePath` ← src/wiki-engine/core/wiki-protocol.ts:174 [EXTRACTED]
  ```
  export function wikiPagePath(page: Pick<WikiPageDraft, "slug" | "relativePath" | "metadata">): string {
  ```
- `normalizeRelativePagePath` ← src/wiki-engine/core/wiki-protocol.ts:183 [EXTRACTED]
  ```
  export function normalizeRelativePagePath(value: string): string {
  ```
- `wikiLinkTarget` ← src/wiki-engine/core/wiki-protocol.ts:188 [EXTRACTED]
  ```
  export function wikiLinkTarget(relativePath: string): string {
  ```
- `toPosix` ← src/wiki-engine/core/wiki-protocol.ts:192 [EXTRACTED]
  ```
  export function toPosix(value: string): string {
  ```
- `extractToml` ← src/wiki-engine/code-knowledge/extractors/config.ts:12 [EXTRACTED]
  ```
  export function extractToml(files: CodeCollectedFile[]): CodeFact[] {
  ```
- `extractSql` ← src/wiki-engine/code-knowledge/extractors/config.ts:38 [EXTRACTED]
  ```
  export function extractSql(files: CodeCollectedFile[]): CodeFact[] {
  ```
- `extractGo` ← src/wiki-engine/code-knowledge/extractors/go.ts:8 [EXTRACTED]
  ```
  export function extractGo(files: CodeCollectedFile[]): CodeFact[] {
  ```
- `extractJava` ← src/wiki-engine/code-knowledge/extractors/java.ts:8 [EXTRACTED]
  ```
  export function extractJava(files: CodeCollectedFile[]): CodeFact[] {
  ```
- `extractPython` ← src/wiki-engine/code-knowledge/extractors/python.ts:9 [EXTRACTED]
  ```
  export function extractPython(files: CodeCollectedFile[]): CodeFact[] {
  ```
- `extractRust` ← src/wiki-engine/code-knowledge/extractors/rust.ts:8 [EXTRACTED]
  ```
  export function extractRust(files: CodeCollectedFile[]): CodeFact[] {
  ```
- `extractTypescript` ← src/wiki-engine/code-knowledge/extractors/typescript.ts:8 [EXTRACTED]
  ```
  export function extractTypescript(files: CodeCollectedFile[]): CodeFact[] {
  ```