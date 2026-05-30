# Contributing to INORSA

Thank you for contributing. These guidelines apply to all repositories in the INORSA organization unless a specific repo provides its own `CONTRIBUTING.md`.

## Branches

- `main` is the default branch for all repositories.
- Use descriptive branch names: `feature/<short-description>`, `fix/<short-description>`, or `chore/<short-description>`.
- Release branches follow the pattern `release/*`.
- Do not push directly to `main` — all changes go through pull requests.

## Commits

We encourage [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` — a new feature
- `fix:` — a bug fix
- `chore:` — maintenance, tooling, or housekeeping
- `docs:` — documentation updates

Keep commits atomic and focused on a single change.

## Pull requests

- Fill out the PR template (What / Why / Testing / Checklist).
- Squash merge is the preferred merge strategy (merge commits are disabled org-wide).
- Request review from the appropriate code owners. Each repository should have a `.github/CODEOWNERS` file — check that file for the right reviewers.
- Ensure CI passes before requesting review.

## Labels

Labels are standardized across the org via [org-management](https://github.com/INORSA/org-management). Use these when filing issues:

| Label | Use for |
|-------|---------|
| `type:bug` | Something is broken |
| `type:feature` | New feature or capability |
| `type:chore` | Maintenance or housekeeping |
| `type:docs` | Documentation updates |
| `type:security` | Security-related changes |

Priority labels (`priority:critical`, `priority:high`, `priority:medium`, `priority:low`) help triage.

## Stale PR policy

PRs with no activity for 30 days receive a `stale` label. After 7 more days they are automatically closed. To prevent auto-closure, add one of these exemption labels:

- `keep-open` — explicitly keep this PR open indefinitely
- `blocked` — blocked on an external dependency
- `awaiting-review` — waiting for review
- `pinned` — important PR that must remain open

Any activity (comment, commit, review) removes the `stale` label and resets the timer.

## Development setup

Refer to each repository's own README for environment setup, dependencies, and build instructions.

## Code style

Follow the linters and formatters configured in each repository. When no specific tooling is configured, follow the language's community conventions.

## Security

If you discover a security vulnerability, **do not open a public issue**. See [SECURITY.md](SECURITY.md) for responsible disclosure instructions.
