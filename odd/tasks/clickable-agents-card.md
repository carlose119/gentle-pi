# Clickable Agents card in the contribution fork

## Objective
Let users click a visible Agents task row in fullscreen mode to open the existing live details view with that task selected. Develop and review the proposal in `carlose119/gentle-pi`, then reference the fork-local PR on upstream `Gentleman-Programming/gentle-shell#1655`.

## Scope and authority
- User explicitly authorized enabling fork Issues, preparing an issue for their approval, implementation/tests, commits, publishing a fork-local PR, and commenting its link upstream.
- Fork approval does not approve the upstream issue. No upstream PR, merge, release, or changes in gentle-ai are authorized.
- Protected approval requires a fresh exact issue-number instruction and verified approver identity/authority. First-person issue form statements require explicit affirmation.
- One writer; preserve normal terminal selection/scrollback, keyboard access, clipping/overflow, resizing, and live task/thread identity.
- Implementation branch: `feat/clickable-agents-card`, created after fork issue approval from `7a27c1c008b3922b851da5efb78e4ca4dae6e6b1` before source writes. Fork issue: https://github.com/carlose119/gentle-pi/issues/1.

## Tasks
- [x] T1 — Enable fork Issues, publish the reviewed feature issue, and obtain explicit verified approval.
  Route: parent handles bounded GitHub administration/publication; explorer maps forms/policy (mandatory mapping trigger).
  Checks: exact repository readback, completed open-and-closed duplicate search, reviewed YAML-form answers, privacy scan, exact issue readback, approval authority and label readback. Close with a tracking work-unit commit on the feature branch after approval.
- [ ] T5 — Resolve the local test-runner prerequisite without unrelated source or fork changes.
  Route: bounded delegated setup worker; user explicitly authorized declared local dependency installation. Only generated `node_modules/**` may change (including scoped npm/pnpm caches there). Do not change source, manifests/lockfiles, global Pi, or fork branches. Inspect symlinks before writing to avoid escaping local scope.
  Checks: verify declared dependency versions/resolution, reproduce exact baseline failure, establish deterministic focused baseline readiness, preserve manifests/lockfiles/branch/fork, report any remaining limitations. Close with tracking/config work-unit commit after outcome observed.
- [ ] T2 — Implement fullscreen click-to-details as one coherent behavior work unit with regression tests.
  Route: one gentle-ai-worker (mandatory multi-file writer trigger); self-verification, native review according to the user-owned switch, and ASSESS-directed independent verification as needed.
  Checks: observed RED/GREEN/refactor; task row hit geometry, non-task and overflow exclusions, initial selection, keyboard/default behavior, resize-stale geometry, live thread identity, focused suite and applicable full suite/build. Close with a Conventional Commit containing behavior, tests, and applicable docs.
- [ ] T3 — Publish a fork-local PR from the feature branch to fork main.
  Route: parent publishes under explicit authorization; delegate expensive verification when needed.
  Checks: approved fork issue linked, exactly one existing type label, truthful checks, base/head/target readback, review-size assessment. Record URL and work-unit evidence.
- [ ] T4 — Comment on upstream issue 1655 with the verified fork PR link and test results.
  Route: parent contextual publication under explicit authorization.
  Checks: target issue identity, privacy scan, one comment attempt, exact comment readback; do not modify upstream labels. Record comment URL and work-unit evidence.

## Implementation surfaces
- `lib/agents-widget.ts`
- `lib/agents-view.ts`
- `extensions/gentle-agents.ts`
- `tests/agents-widget.test.ts`
- `tests/agents-view.test.ts`
- `tests/gentle-agents.test.ts`
- `docs/gentle-shell.md` (concise fullscreen click instructions only)

Existing `tests/agents-view-thread-identity.test.ts` is an important regression check, not currently an authorized edit surface. Expand only when mapping justifies it. Documentation changes remain conditional on actual user-facing instructions.

## Evidence and progress
- Read-only explorer `murab40f-1-xo9g` completed: existing AgentsView can be reused; widget needs render-derived hit geometry and fullscreen event wiring.
- Fresh host readback: authenticated account `carlose119` (id 29585287), fork permission ADMIN, default branch main, parent Gentleman-Programming/gentle-shell.
- Issues enabled by one authorized `gh repo edit` attempt; exact host readback confirmed `hasIssuesEnabled: true`.
- Completed fork open-and-closed issue listing (limit 1000): empty, unsaturated; no duplicate.
- Remote feature form blob equals local form blob (`e28d9f8e28a3b9c0c9f933a9da947d1abbf603b4`). Required first-person search/privacy statements need fresh affirmation for this fork.
- Owner explicitly confirmed identity as carlose119 and separately authorized creating `status:needs-review`, `status:approved`, and `type:feature` as fork configuration. One create attempt per label and host readback confirmed all three. No approval was applied. Existing `enhancement` plus `status:needs-review` are the selected form's permitted create-time labels.
- Local main was clean before creating this tracking document. Feature branch now exists; source implementation, PR, and upstream comment are not yet present.
- User explicitly confirmed reviewed fork issue draft and both required first-person declarations via `confirm_fork_issue`.
- Initial publication invocation returned exit 0 and no result output. Separate read-only verifier `murb3gr9-2-q60s` reproduced the exact multiline stdin parsing shape and established that the outer try block never executed: no publication attempt/no_write. Inserting a blank line after finally executed all harmless sentinel outputs. Parent supplied original exact closing bytes; all temp setup and gh issue create were inside the unexecuted block. Host issues `[]` and zero temp dirs corroborate but do not independently establish this classification.
- Corrected stdin invocation first emitted no_write at private-temp-setup: Get-Acl/Set-Acl were unavailable. Read-only follow-up `murb91qo-3-i3jp` verified .NET ACL methods. Final invocation used secure DirectoryInfo.Create(DirectorySecurity), explicit FileSecurity on five files, and validated protected owner-only FullControl permissions before writing body-bearing data; cleanup completed without error. No installation or privacy weakening.
- First actual gh issue create succeeded: https://github.com/carlose119/gentle-pi/issues/1, OPEN; exact title/body/identity/state/labels readback matched confirmed draft. Outcome confirmed.
- User explicitly approved exact fork issue 1. Fresh principal carlose119 and ADMIN permission verified; one atomic approval operation added `status:approved`, removed `status:needs-review`, preserved `enhancement`, and exact pre/post readback confirmed. Private snapshots cleaned. No upstream approval claimed.
- T1 complete: setting/form/hash/duplicate/private ACL/privacy/exact publication/atomic approval checks passed; tracking work-unit commit `cd1ae762b0f0c48ad33145d8a793c0d1646ffb48` observed on the feature branch. Tests/build/native review are not applicable to this administrative plus passive tracking unit; no meaningful RED exists.
- T2 paused/pending: completed writer made no edits; test-runner prerequisite must resolve before focused RED/production implementation/GREEN/refactor/full checks. T5 is in progress; user explicitly authorized bounded declared local dependency setup with no global installation or source/manifest/lockfile/branch changes.
- Writer `murbk6k8-4-97fj` finished partial after parent pause; files_changed `[]`. Runtime: node v22.23.2; pnpm command not found. Focused baseline: 51 tests passed, 1 module-load failure because installed `@earendil-works/pi-tui` does not export existing `colorToRgb` import. This is pre-existing; no RED/GREEN/refactor or behavior candidate exists. Full suite/build/manual fullscreen/native review not run.
- Read-only verifier `murbm7r2-5-867y` resolved ancestry: fork main `1f345106ff2931383451d4e05ec76d1259471884` is five commits ahead of feature baseline `7a27c1c008b3922b851da5efb78e4ca4dae6e6b1`, with zero unrelated baseline diff files in prospective fork PR. No fork synchronization demonstrated necessary; preserve both branches. RDD freshly on (global), clone-local unset.

## Verification commands
Focused candidate command from exploration:
`node --experimental-strip-types --test tests/agents-widget.test.ts tests/agents-view.test.ts tests/agents-view-thread-identity.test.ts tests/gentle-agents.test.ts`

Full suite uses `scripts/run-test-suite.mjs`; verify package scripts/runtime before running. Never claim suite/build success from source inspection.

## Next step
Bounded T5 setup worker `murbv9cn-6-iu59` is running with generated node_modules-only surfaces and exact install/focused-check commands. Preserve declared versions, manifests/lockfiles, global Pi, and both branches; stop if wider changes are needed. T5 in progress; T2 paused/pending with no source edits; T1 complete; T3–T4 pending. Mirror: `odd/clickable-agents-card/tasks`.
