# Agent State

Portfolio upkeep, 2026-09-11. Working from deployed/main d3c1fa8 in an isolated
checkout; preserve the original checkout's existing .gitignore edit.

Task list for this pass:
- [x] Map production and reproduce focused-button keyboard failures.
- [x] Confirm all 1,425 question records and the missing 107-card Perspective category.
- [x] Repair keyboard handling, semantic controls and complete category selection.
- [x] Apply the Prawn Projects visual style, self-host the font and reduce unused UI code.
- [x] Verify type checking, deck transitions, browser workflows, preserved data and build size.
- [x] Release to production and verify both public aliases against the exact commit.

This is a static browser game with no backend, account flow or persistent saves.
Keep question data intact. Review source and production evidence before claiming
the broader portfolio, free-tier or UI requirements complete.

Local evidence: fourteen unit checks, the first twenty-four browser scenarios,
and six final layout/catalog checks passed at 1440, 390 and 320 pixels.
All 1,425 prompts fit the revealed card; the question file is unchanged.
Type checking and production build pass. JavaScript is about 25.7% smaller;
the dependency audit reports zero known vulnerabilities. The same full suite
of twenty-seven browser checks passed in PR and main CI on Node 24.

Released via PR #206 at 5790271d1fc9a50558bb0cede02a1716484a72ab.
Vercel deployment dpl_59TS5XWtpmbVGhToM4Az1YkCQRVs is READY; both public aliases
serve all six files byte-identical to the main CI artifact. The primary alias
passed all twenty-seven browser scenarios; the custom alias passed three focused
keyboard/theme/layout checks. GitHub marked the browserslist advisory fixed.
Original question bytes and the user's local ignore rules are preserved.

This focused game repair is complete. Continue the portfolio rotation; shared
workflow hygiene and broader free-tier measurements remain open. This static
app has no cloud polling or persistent saves. Bundle size is not a measurement
of monthly savings. Keep production evidence linked to the source release above;
subsequent documentation-only commits do not change its application files.

2026-09-12: opt in to the shared activity-branch heartbeat. Weekly repository activity moves to automation/heartbeat, which Vercel is configured not to deploy. Normal app branches keep deploying. Local and hosted validation, production release, and first manual heartbeat verification are pending. The 60-day inactivity behavior requires longer observation. No application data or collection schedules are changed.

2026-09-12 heartbeat validation passed locally. Source policy tests and workflow parsing pass; the application pilot builds pass. Hosted PR checks, production matching and the first branch heartbeat are the next release gates. No broad sync or disabled workflow reactivation was run.

2026-09-12 required-check rollout task list: verify current production and workflows; consolidate unit/type/build and browser validation under Build on every PR/main update; install the shared exact-head bot policy while leaving its workflows disabled; repair shared protected-branch config PRs; verify hosted releases before configuring required Build/Vercel checks; verify blocked and passing PR behavior plus heartbeat compatibility and update the portfolio report. The heartbeat pilot is already released. This patch changes validation/maintenance configuration only; application source, dependency versions, question records and Vercel asset configuration remain unchanged. Older app-check workflows are retained for manual diagnostics. Required branch checks and bot reactivation have not yet been configured.

2026-09-12 local validation passes: locked install, 14 unit tests and 27 browser scenarios, type checking and production build. Application code, data, dependencies and Vercel configuration are byte-preserved. The shared checked bot policy is installed but its workflows remain disabled; required Build/Vercel rules will be enabled only after hosted and production verification. Default CodeQL completion is included in the policy triggers.
