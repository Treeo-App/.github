# Security policy

## Reporting a vulnerability
If you find a vulnerability in any Treeo-App repository, do not open a public issue or mention it in a PR. Report it privately using the **Security > Report a vulnerability** option of the affected repository, or send a private message to the project maintainer (@erikodes).

We aim to acknowledge reports within a few days and keep the reporter informed until the issue is fixed.

## Secrets and sensitive data
Credentials, service account keys, signing certificates, tokens and `.env` files are never committed. If a secret is accidentally exposed, it must be rotated immediately and the maintainer notified.

## Branch workflow
Every change goes through a Pull Request into `develop`. The `main` branch represents production and only receives PRs from `develop`.
