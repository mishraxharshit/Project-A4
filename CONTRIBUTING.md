# Contributing to Project-A4

Thank you for your interest in contributing to Project-A4 (Cognitive Engineering & Research). This document explains how to propose changes, report issues, and get your contribution merged.

## Ways to Contribute

- **Research**: literature notes, experiment write-ups, critiques, replications
- **Code**: reference implementations, tooling, bug fixes, performance improvements
- **Documentation**: clarifying docs, tutorials, examples
- **Community**: triaging issues, reviewing PRs, answering questions

## Before You Start

1. Check open [issues](../../issues) and [pull requests](../../pulls) to avoid duplicate work.
2. For substantial changes (new sub-project, architecture change, new research direction), open an issue first to discuss scope before investing significant time.
3. Read the [Code of Conduct](CODE_OF_CONDUCT.md).

## Development Workflow

1. **Fork** the repository and create your branch from `main`:
   ```bash
   git checkout -b feat/short-description
   ```
2. Make your changes, keeping commits focused and descriptive.
3. If your change affects `/src`, add or update tests under `/tests`.
4. If your change affects research content, place it under `/research` with a clear filename and a short header describing scope, date, and status (draft/final).
5. Run any available checks/linters locally before opening a PR (see `/scripts` once available).
6. Open a pull request against `main` using the PR template. Link related issues.

## Commit Messages

Use clear, imperative-mood commit messages, e.g.:

```
Add benchmark harness for memory-retention experiments
Fix off-by-one error in tokenizer boundary check
Document architecture decision on evaluation pipeline
```

Conventional Commits style (`feat:`, `fix:`, `docs:`, `research:`, `chore:`) is encouraged but not yet enforced.

## Code Review

- All contributions require review from at least one maintainer before merge.
- Be responsive to review feedback; if you disagree, explain your reasoning — reviews are a discussion, not a gate.
- Maintainers may request changes for security, licensing, or research-integrity reasons non-negotiably (see [`SECURITY.md`](SECURITY.md)).

## Research Contribution Standards

To keep research content trustworthy:

- Cite sources for claims and prior work.
- Clearly separate original findings from summaries of external work.
- Disclose any conflicts of interest or funding sources relevant to submitted research.
- Mark experimental/unverified claims as such.

## Licensing of Contributions

By submitting a contribution, you agree that it will be licensed under the same license as the repository (see [`LICENSE`](LICENSE)), unless explicitly and clearly stated otherwise in the contribution itself.

## Questions

Open a [Discussion](../../discussions) or an issue tagged `question`.
