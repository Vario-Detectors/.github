# Contributing

These are the default contribution rules for Vario Detectors repositories. A repo may add its own `CONTRIBUTING.md` on top of this.

## Pull requests

- One task per branch and pull request.
- Branch names: `feat/…`, `fix/…`, `chore/…`, and similar.
- Draft PRs are welcome.
- Do not merge without Ömer's approval.
- Do not force-push or rewrite history on shared branches.
- Do not skip git hooks (`--no-verify`).

## Commits

- Short, imperative subject lines (Conventional Commits style is fine).
- Example: `fix: clear Alt latch when the editor loses focus`

## Quality

- Start bug fixes from a **scenario matrix**: a table of inputs and expected results (table-driven tests covering many cases). Fix until every row passes.
- Prefer tests of behavior over tests of implementation.
- Make the smallest change that works. Subtract before you add.
- Prove it works before you claim it is done: tests, a build, or a real run. Put that verification evidence in the PR.

## Android

- Package / `applicationId` prefix is `com.meowgi.<app>` unless the product says otherwise. If a company product should use a different vendor prefix, ask Ömer — do not invent one.
- On every delivered build, bump both `versionName` and `versionCode`. Never reuse a `versionCode`.

## Secrets

Never commit secrets, keystores, or passwords. That includes `.env` files, `*.jks`, `*.keystore`, API keys, and similar. Keep keys outside the repository.

## Time

Use Europe/Istanbul and a 24-hour clock in commits, PRs, issues, and docs when you mention a time.
