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
- [x] T5 — Resolve the local test-runner prerequisite without unrelated source or fork changes.
  Route: bounded delegated setup worker; user explicitly authorized declared local dependency installation. Only generated `node_modules/**` may change (including scoped npm/pnpm caches there). Do not change source, manifests/lockfiles, global Pi, or fork branches. Inspect symlinks before writing to avoid escaping local scope.
  Checks: verify locked installation/resolution, preserve manifests/lockfiles/branch/fork, establish runnable core/UI baseline and exact attribution of any base-only failures. A passing combined suite is not claimed; exact pre-existing failures are documented and excluded only from candidate regression accounting, not hidden or fixed. Close with a tracking/config work-unit commit after observed installation/core/ledger evidence.
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
- T5 complete for locked dependency setup/runnable baseline attribution with tracking work-unit commit `ff278a44e3a15c4ebe04dcc16d4fbf2240801e2e`. Installer/runtime/core/integrity/known-base ledger checks observed. The combined suite still has the exact 23 reported pre-existing failures; no clean-suite claim or unrelated fix.
- T2 source implemented by settled writer `mure5rth-9-6i69`: seven allowed files, 160 additions/14 deletions. Meaningful RED observed for initial task selection and production widget click wiring; GREEN core 53/53 and filtered production click/pointer/footer 3/3. Four optional-terminal regressions corrected during triangulation/refactor. Combined suite: 203 pass, exact 23 known base failures; not green.
- T2 remains partial: full runner timed out after 600 seconds in unit stage, with additional unclassified SDK discovery timeout, launcher missing cmd.exe, symlink permission failures, assertions/cancellations. No final totals or later stages observed. Real-terminal fullscreen unavailable; synthetic production wiring verified. Manifests/lock hashes unchanged, diff check passed.
- Independent verification confirmed core 53/53, filtered production 3/3 (unmatched omitted), types ratchet 187 baseline diagnostics/no regressions, runtime check eight modules match, manifest integrity and whitespace checks. Isolated SDK discovery 1/1 passed in 5.499 seconds; this does not establish full-suite success. Additional symlink/chmod fixture failures have unchanged-base evidence; cancellations remain unresolved.
- Native behavior review approved and exact acknowledgement burned authority for target `sha256:d95d7e8040622a1562fdaafc80719bddf103eda146f034c124269214fd8e4898`, lineage `review-87fb20a3e58b6c4e`, consumed revision `sha256:287a1c8724145c986f5475967c92b06b16f63ba434500a3635794b017fb8e452`. Reviewed slice checkpoint commit `84ec2468946abcbdfc347831fc258391fc19adc4` observed; this is not a clean-suite or T2-completion claim. Earlier passive task dispatch checkpoint: `d471b7da9bdfaca963dc98d32c26cd8ac9e7187c`.
- Read-only verifier continuation `murfkclz-b-yijx` is reproducing one explicitly authorized SIGINT provisioning cancellation case. No code remediation, cleanup, or publication authorized by review outcome; full workflow publication remains pending required verification disposition.
- Writer `murbk6k8-4-97fj` finished partial after parent pause; files_changed `[]`. Runtime: node v22.23.2; pnpm command not found. Focused baseline: 51 tests passed, 1 module-load failure because installed `@earendil-works/pi-tui` does not export existing `colorToRgb` import. This is pre-existing; no RED/GREEN/refactor or behavior candidate exists. Full suite/build/manual fullscreen/native review not run.
- T5 setup worker `murbv9cn-6-iu59` finished interaction_required: pnpm11.1.1 downloaded into local npm cache, but installation stopped with `ERR_PNPM_ABORTED_REMOVE_MODULES_DIR_NO_TTY`. Existing Pi tui/ai/coding-agent0.85.1 remain; lock selects1.0.0 and colorToRgb remains undefined. No baseline rerun after failed install. Node_modules local/no escaping symlinks; manifest/lock hashes unchanged (`8cb0b729826fb4070f4e69497e89aa7bca324995`, `e4d9a3c843b923536edcb4c40d0f69a18741f232`). No source/global changes.
- User explicitly authorized child envelope's exact `CI=true` scoped installer retry. Setup worker `murdgfbk-7-cyqo` completed partial: locked installation passed (187 packages), local Pi packages now 1.0.0 and colorToRgb is a function; only generated dependencies/caches changed, with no escaping symlinks or manifest/lock changes. Focused baseline now ran 223 tests: 200 passed, 23 assertion failures (2 diff-relay, 5 mutation-attribution, 1 spawn-environment, 15 writer-admission). Root causes remain unverified; no feature edits or feature RED/GREEN.
- Settled independent verifier `murds7bk-8-rpo1`: combined 223 total, 200 pass/23 fail, exit 1; independent core 51/51, exit 0; existing production pointer composition/footer tests pass. Integrity cleared: parent-owned tracking update only, source/tests/manifests unchanged. Seven slash-prefix stub failures and sixteen ancestor-repository fixture failures have source/diagnostic support; no counterfactual fixture edits or safety variable changes were performed. Feature TDD can run meaningfully without unrelated fixes.
- Tracking review d79b80c3 approved/acknowledged: lineage `review-67955e9935fdc950`, consumed revision `sha256:c45f1baf0a8350ccaced91b5f848bef7f4d25511bfa3de243026191c11f2665c`; authority burned. This covers prior six-line tracking slice only, not later evidence updates or future behavior.
- Tracking-only native review for prior exact target `sha256:98d342987ee082bae81c6bf8225f8fd4dd500046ba0a02f553138dc3fbc61e96` approved/acknowledged; lineage `review-fea899ba76e3a95b`, consumed revision `sha256:5c0b49ad60ec185d3d81a817c0e6374402413a5a016b6e5a6f1757c84cad516c`, authority burned. That prior tracking slice committed as `a3baea6ab4eb13fae7f2f875023c47d0c857f5c2`; it does not review later tracking edits or future behavior.
- Read-only verifier `murbm7r2-5-867y` resolved ancestry: fork main `1f345106ff2931383451d4e05ec76d1259471884` is five commits ahead of feature baseline `7a27c1c008b3922b851da5efb78e4ca4dae6e6b1`, with zero unrelated baseline diff files in prospective fork PR. No fork synchronization demonstrated necessary; preserve both branches. RDD freshly on (global), clone-local unset.

## Verification commands
Focused candidate command from exploration:
`node --experimental-strip-types --test tests/agents-widget.test.ts tests/agents-view.test.ts tests/agents-view-thread-identity.test.ts tests/gentle-agents.test.ts`

Full suite uses `scripts/run-test-suite.mjs`; verify package scripts/runtime before running. Never claim suite/build success from source inspection.

## Next step
Await settled cancellation/full-check disposition from `murfkclz-b-yijx`. Source is checkpointed and native review closed; do not mark T2 complete or publish while required verification remains unresolved. No unrelated fixes or forced full-suite success. T5/T1 complete; T2 in progress/partial; T3–T4 pending. Mirror: `odd/clickable-agents-card/tasks`.

## Known pre-existing Windows baseline failures
The combined command fails on these 23 exact tests in `tests/gentle-agents.test.ts` BEFORE any feature edit. Never call the combined suite green; only these matched base failures may be excepted from candidate regression accounting. Any new failure remains blocking.

Slash-prefix fake resolvers (Windows backslash descendants fail forward-slash containment; baseline lines 1518,1868,1902,1939,1975,2010):
- owned child diff relay validates the exact file independently of review bookkeeping: true
- owned child diff relay validates the exact file independently of review bookkeeping: false
- a mutation dropped for lacking any session-change evidence explains itself once
- a mutation dropped for evidence pointing at a different worktree root explains itself once
- a mutation dropped for an unreadable evidence target explains itself once
- a mutation dropped for mismatched session-change evidence explains itself once
- a successfully attributed mutation adds no drop note

Nominal non-Git temporary fixtures enclosed by an ancestor repository:
- default Node spawn adapter distinguishes IPC-only and permission-capable canonical Git children
- bounded writer executor admission before bootstrap: implicit-worker
- bounded writer executor admission before bootstrap: explicit-worker
- bounded writer executor admission before bootstrap: implicit-gentle-ai-worker
- bounded writer executor admission before bootstrap: explicit-gentle-ai-worker
- bounded writer executor admission before bootstrap: model
- bounded writer executor admission before bootstrap: profile-model
- bounded writer executor admission before bootstrap: profile-valid
- bounded writer executor admission before bootstrap: foreign
- bounded writer executor admission before bootstrap: nested
- bounded writer executor admission before bootstrap: missing
- bounded writer executor admission before bootstrap: off
- bounded writer executor admission before bootstrap: shutdown
- bounded writer executor admission before bootstrap: replacement
- bounded writer executor admission before bootstrap: changed-id
- bounded writer executor admission before bootstrap: during-cancel

No source fixes or ancestor-repository changes authorized. Existing production pointer/footer checks and core baseline pass. Real-terminal fullscreen behavior remains unverified.
