# .github

This repo contains org-wide defaults for all repositories in this GitHub org.

## What's in here

| File/Folder | Purpose |
|---|---|
| `profile/README.md` | Public org profile shown on GitHub |
| `PULL_REQUEST_TEMPLATE.md` | Default PR template for all repos |
| `ISSUE_TEMPLATE/bug_report.md` | Bug report template |
| `ISSUE_TEMPLATE/feature_request.md` | Feature request template |
| `ISSUE_TEMPLATE/capability_extraction.md` | Template for flagging reusable logic to extract |
| `CONTRIBUTING.md` | Contribution guidelines for all repos |

---

## How GitHub uses this repo

GitHub automatically applies the templates and guidelines here as **org-wide defaults**.  
Individual repos can override these by creating their own `.github/` folder locally.

---

## Updating these files

Any change here affects **all repos in the org** — treat PRs to this repo with care.

- CHANGE TO `CONTRIBUTE.md` or `PULL_REQUEST_TEMPLATE` affect every contributor immediately.
- Change to `profile/README.md` affect the public face of the org.
- When in doubt, discuss before merging