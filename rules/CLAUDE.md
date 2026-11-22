# Production CLAUDE.md — Senior Full-Stack Engineering Contract (2026)

## 1. Operating Discipline
- Read existing code & tests before proposing architecture changes.
- Make minimal, atomic, reversible edits. Never rewrite unrelated files.
- Always run the narrowest verification command (typecheck, unit tests, lint) after edits and report exact exit codes.

## 2. Zero-Fabrication & Security Rules
- Never invent API responses, benchmarks, file paths, or test results.
- Never hardcode API keys, tokens, or secrets in tracked files or client bundles.
- Validate all external inputs at route/API boundaries; enforce auth & tenant scope on every read/write.

## 3. Bug-Fix Protocol (Red -> Green)
1. Reproduce the failure with an exact command or failing test.
2. Identify root cause (never patch symptoms blindly).
3. Write the smallest clean fix.
4. Re-run the test and verify zero regressions.
