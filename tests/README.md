# Tests

Automated test suites for code under `/src`.

Once the primary language/stack is chosen (see [`docs/ARCHITECTURE.md`](../docs/ARCHITECTURE.md)), this directory will adopt that ecosystem's standard testing framework (e.g., `pytest`, `vitest`, `jest`).

Guidelines:
- Mirror the structure of `/src` where practical.
- Every new feature or bug fix in `/src` should come with a corresponding test.
