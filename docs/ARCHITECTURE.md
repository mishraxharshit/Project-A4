# Architecture

> This document will grow as technical decisions are made. It currently captures the intended shape of the ecosystem rather than a finished design.

## Design Principles

1. **Research and engineering are peers.** Neither `/research` nor `/src` is secondary — the repo layout keeps both visible and equally maintained.
2. **Reproducibility first.** Experiments, benchmarks, and results should be re-runnable by others, not just described.
3. **Composable over monolithic.** Favor small, well-documented components over one large undifferentiated codebase, so pieces can later graduate into their own repositories.
4. **Safety and provenance.** Data sources, model provenance, and licensing are tracked, not assumed.

## Open Decisions

These are intentionally left open until the community/maintainers converge on them — track discussion in linked issues:

- [ ] Primary implementation language(s) for `/src`
- [ ] Packaging / distribution strategy (e.g., PyPI, npm, standalone)
- [ ] Data storage and versioning approach for datasets under `/research`
- [ ] Documentation site generator (e.g., MkDocs, Docusaurus) vs. plain Markdown
- [ ] Release cadence and versioning scheme

## High-Level Component Map

```
┌─────────────────────────────┐
│           docs/             │  Architecture, roadmap, decisions
└─────────────┬────────────────┘
              │
┌─────────────┴────────────────────────────────────────┐
│                     Project-A4 (hub)                  │
│                                                        │
│   research/       src/          examples/   tests/    │
│   (papers,        (reference    (usage      (test     │
│   experiments,    implementa-   demos)      suites)   │
│   notes)          tions)                              │
│                                                        │
│   tools/          scripts/                            │
│   (dev/research   (automation,                        │
│   tooling)        setup)                               │
└────────────────────────────────────────────────────────┘
```

As components mature, they may be extracted into dedicated repositories under the same organization, linked back from this hub.
