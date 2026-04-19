# AGENTS.md

Purpose: keep changes small, safe, test-first, and easy to refactor.

## Rules
- Prefer TDD: write or update a failing test first, then implement, then refactor.
- Do one feature or bugfix at a time. Avoid unrelated changes.
- Keep commits and GitHub pushes small, consistent, and easy to review.
- Prefer simple, composable code. Avoid premature abstraction.
- Keep the code adaptable: centralize shared logic, remove duplication, and make reuse easy.
- Export shared design tokens for common colors, headings, spacing, and similar styles.
- Security first: validate input, handle secrets carefully, avoid unsafe parsing or eval, and do not weaken existing protections.
- Keep tests green; add regression tests for every fix.
- Before handoff, run the relevant tests and note any remaining risk.

## Workflow
1. Inspect the codebase and match existing patterns.
2. Write one failing test.
3. Implement the smallest change that passes.
4. Refactor only after tests pass.
5. Verify with targeted tests.
6. Commit and push only when the single feature is complete.

## Style
- Follow local conventions.
- Prefer explicit names, small functions, and clear boundaries.
- Do not add new dependencies unless necessary.

## Output
- Summarize what changed.
- List tests run.
- Call out follow-up work only if needed.
