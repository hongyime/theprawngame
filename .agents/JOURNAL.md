# Decision journal

- 2026-09-11: Derive card sets from the preserved question catalog so Perspective and future categories remain playable. Use native keyboard controls, atomic deck transitions, Prawn Projects styling and a local font to repair navigation and remove unused runtime/build dependencies; verify on three viewport sizes before production.
- 2026-09-11: PR #206 released the repair after 14 unit and 27 browser checks. Both production aliases match the main CI artifact; 27 primary-alias and 3 custom-alias browser checks passed. Preserve all question data and the existing local ignore edit; return to the portfolio queue after this bounded release.

2026-09-12: opt in to the shared activity-branch heartbeat. Weekly repository activity moves to automation/heartbeat, which Vercel is configured not to deploy. Normal app branches keep deploying. Local and hosted validation, production release, and first manual heartbeat verification are pending. The 60-day inactivity behavior requires longer observation. No application data or collection schedules are changed.

2026-09-12 heartbeat validation passed locally. Source policy tests and workflow parsing pass; the application pilot builds pass. Hosted PR checks, production matching and the first branch heartbeat are the next release gates. No broad sync or disabled workflow reactivation was run.
