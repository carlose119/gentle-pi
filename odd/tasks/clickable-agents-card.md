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
- [ ] T1 — Enable fork Issues, publish the reviewed feature issue, and obtain explicit verified approval.
  Route: parent handles bounded GitHub administration/publication; explorer maps forms/policy (mandatory mapping trigger).
  Checks: exact repository readback, completed open-and-closed duplicate search, reviewed YAML-form answers, privacy scan, exact issue readback, approval authority and label readback. Close with a tracking work-unit commit on the feature branch after approval.
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
- T1 checks: setting/form/hash/duplicate/private ACL/privacy/exact publication/atomic approval checks passed. Tests/build/native review are not applicable to this administrative plus passive tracking work unit; no meaningful RED exists. Tracking commit still pending.
- No test, build, manual fullscreen, or native review result has been observed. Node/pnpm/dependency readiness still needs verification.

## Verification commands
Focused candidate command from exploration:
`node --experimental-strip-types --test tests/agents-widget.test.ts tests/agents-view.test.ts tests/agents-view-thread-identity.test.ts tests/gentle-agents.test.ts`

Full suite uses `scripts/run-test-suite.mjs`; verify package scripts/runtime before running. Never claim suite/build success from source inspection.

## Next step
Close T1 with the authorized passive tracking work-unit commit, record commit evidence, then start one bounded T2 writer with test-first and exact allowed surfaces. T1 administrative checks passed; commit pending. T2–T4 remain pending. Mirror: `odd/clickable-agents-card/tasks`.
