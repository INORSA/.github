# .github

Organization-wide default community health files, issue/PR templates, and profile README for **INORSA**. GitHub automatically serves these as fallback defaults to every org repository that does not define its own version.

## How inheritance works

When a contributor opens an issue, PR, or views the Community tab in any INORSA repo, GitHub resolves files in this order:

1. The member repo's own `.github/` folder, root, or `docs/` folder.
2. If not found, GitHub falls back to **this repo** (`INORSA/.github`).

This is static file inheritance only — no workflows execute in other repos from here.

> **Important:** If a member repo creates *any* file inside its own `.github/ISSUE_TEMPLATE/` folder, **all** inherited issue templates from this repo are disabled for that repo. GitHub does not merge local and org-level templates — local fully overrides. Only add a repo-level `ISSUE_TEMPLATE/` folder when you intend to replace the org defaults entirely.

## What's in this repo

| File | Purpose |
|------|---------|
| `profile/README.md` | Org landing page rendered at [github.com/INORSA](https://github.com/INORSA) |
| `SECURITY.md` | Vulnerability reporting policy (inherited by all repos) |
| `CONTRIBUTING.md` | Org-wide contributing guidelines |
| `SUPPORT.md` | Where to get help |
| `CODE_OF_CONDUCT.md` | Contributor Covenant code of conduct |
| `PULL_REQUEST_TEMPLATE.md` | Default PR description template |
| `.github/ISSUE_TEMPLATE/` | Bug report and feature request forms, template chooser config |

## Requirements

- This repo **must be public**. Private `.github` repos do not serve defaults to other repositories.
- No PAT or secret is needed — these are static files served by GitHub automatically.
- Labels referenced in issue templates (e.g. `type:bug`, `type:feature`) must exist on this repo. They are synced automatically by the [Org: Sync Labels](https://github.com/INORSA/org-management) workflow.

## Related repos

| Repo | Purpose |
|------|---------|
| [INORSA/org-management](https://github.com/INORSA/org-management) (private) | Automation: stale PR cleanup, branch cleanup, label sync, settings enforcement, security audits, Dependabot sync, new-repo onboarding |
| **INORSA/.github** (this repo, public) | Defaults: community health files, issue/PR templates, org profile README |

The label taxonomy defined in `org-management/config/labels.yml` is the source of truth for labels used in issue templates here.
