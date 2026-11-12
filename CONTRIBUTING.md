# Contributing guide

## Branches
`main` is production: it is protected and only receives PRs from `develop`. `develop` is the integration branch: all PRs go there. Working branches are created from `develop` with the prefixes `feat/`, `fix/`, `chore/`, `docs/` or `refactor/` (for example: `feat/pinned-collections`).

## Workflow
Create your branch from `develop`, make small commits, open a PR against `develop` and wait for the checks to pass. Once `develop` is stable, a PR from `develop` to `main` is opened to release to production.

## Commits
We use Conventional Commits: `feat:`, `fix:`, `docs:`, `chore:`, `refactor:`, `test:`.

## Before opening a PR
Make sure the project checks pass locally (typecheck, tests and build, depending on the repository).

## Security
Never commit credentials, service account keys or `.env` files. Read [SECURITY.md](SECURITY.md).
