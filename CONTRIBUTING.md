# Contributing

These repositories are maintained by the The Stack Hub team. External contributions are not expected unless a repository says otherwise.

## Branches

Create a branch from the default branch (`main` unless the repository says otherwise):

- `feat/<short-name>` — new behaviour
- `fix/<short-name>` — bug fix
- `chore/<short-name>` — maintenance, dependencies, tooling
- `docs/<short-name>` — documentation only
- `refactor/<short-name>` — no intended behaviour change
- `test/<short-name>` — tests only

Do not commit directly to the default branch. Do not force-push shared branches.

## Commits

Use [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: add offline retry for driver sync
fix: correct GST snapshot on reprinted invoices
chore: bump wrangler
docs: update agent runbook
```

Keep the subject imperative and under 72 characters. Explain why in the body when it is not obvious.

## Pull requests

- Open a PR against the default branch and fill in the pull request template.
- Request review from at least one other teammate before merging.
- Keep the diff focused. Link the issue if there is one.
- Do not merge your own PR unless the team has agreed an exception (for example a trivial typo on a non-production branch).

## Secrets and credentials

Never commit secrets, API keys, tokens, private keys, `.env` files, or credentials. Use repository or environment secrets for CI, and local env files that are gitignored. If a secret is committed, rotate it immediately and report it under [SECURITY.md](SECURITY.md).
