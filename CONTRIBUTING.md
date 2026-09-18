# Contributing to Omotai

Thanks for your interest! Please read this before opening an issue or pull request.

## Scope first

Each repository's README lists its goals and **non-goals**. Requests outside the scope will be closed with a pointer to that list; it keeps the project small enough to maintain and to reason about securely.

## Most wanted: attack scenarios

The single most valuable contribution is a new attack against web agents for the [eval](https://github.com/omotai/eval) suite. Open an issue with the **Attack scenario** template first so we can discuss it before you build it.

## Changes to the security model

Anything that changes what the runtime guarantees (policy semantics, vault behavior, network guard rules, audit format) starts as a short written proposal in an issue using the **Proposal** template. Code comes after agreement.

## Pull requests

- Keep PRs small and focused; one change per PR.
- Add or update tests. CI must pass (`ruff` + `pytest`).
- Never commit secrets. Use `.env` locally (it is git-ignored) and update `.env.example` when adding a variable.
- Tests that call LLM APIs must be marked and skipped in CI; they run locally only.

## Development setup

We use [uv](https://docs.astral.sh/uv/):

```bash
uv sync
uv run ruff check .
uv run pytest
```

## Conduct

By participating you agree to follow our [Code of Conduct](https://github.com/omotai/.github/blob/main/CODE_OF_CONDUCT.md).
