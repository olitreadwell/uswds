# uswds/uswds context
> refreshed 2026-09-04 | upstream default: develop @ 9173c1107

## Identity & policies
- upstream: uswds/uswds, default branch `develop`, primary language JS/TS/Sass/HTML (USWDS design system). English-first: yes.
- CLA/DCO: none (no CLA bot, no DCO/sign-off requirement found in CONTRIBUTING or .github).
- AI-assisted PR policy: unstated (no AI ban/disclosure line found in CONTRIBUTING or org .github).
- signed commits required: YES — CONTRIBUTING.md "Setting up verified commits" ("all commits to this repository must have a verified signature") + `.github/workflows/verify-commit-signatures.yml` (pull_request_target, flags unverified commits). **BLOCKER for automation: no signing key in this environment; config known_blockers.signed_commits names this repo -> outcome `blocked-needs-signing`.**
- PR template: `.github/PULL_REQUEST_TEMPLATE.md` (Summary / Breaking change / Related issue / Related PRs / Preview link / Problem statement / Solution / Major changes / Testing and review). CONTRIBUTING also requires a release-notes statement + "How to Test" section.
- external tracker: github.

## Conventions (verified from merged PRs)
- branch naming: mixed — `fix/`, `bug/`, `feature/`, `docs/`, `automated/`, `release-*`; no strict single convention.
- test/lint: `npm run lint` (eslint + sass-lint), `npm run prettier`, `npm test`; CI gates on these.
- outside PRs get merged; repo is responsive (recent merges daily, e.g. #6843 2026-09-03).

## Maintainer picture
- Active maintainers (USWDS team, GSA/TTS). Responsive; daily merges observed.
- In-flight areas: accessibility skill work (#6749 merged 2026-09-03), combo-box voiceover bug (#6840), date-picker keyboard/touch work.

## Issue-area health
- Accessibility is an active, well-tended area (dedicated `.agents/skills/uswds-accessibility`).
- Modal `aria-describedby` typo: upstream issue #5652 still open, but fix already proposed upstream by PR #6755 (open, head `fix/modal-aria-describedby-typo`) — DO NOT re-pick.

## Gap ledger (dedupe — READ FIRST, never re-pick)
- `2026-09-04` self-found trivial fixes (calender->calendar in usa-date-picker/src/index.js:1755; broken `http://CHANGELOG.md` link in GOVERNANCE.md:55) — outcome: **blocked-needs-signing** — repo requires verified commits; automation has no signing key and must not register one to Oli's account. No PR opened. Unlocks if Oli registers an SSH/GPG signing key on his GitHub account.

## Mined gaps (discovered, not yet attempted)
- `2026-09-04` usa-date-picker/src/index.js:1755 comment typo `calender`->`calendar` — status: proposed (blocked on signing).
- `2026-09-04` GOVERNANCE.md:55 broken link `http://CHANGELOG.md` (no CHANGELOG.md in repo) — status: proposed (blocked on signing).
