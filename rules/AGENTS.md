# Multi-Agent AGENTS.md Governance Template (Antigravity / Codex / Claude Code)

## Scope & Ownership
- Keep domain logic inside its owning module; shared helpers expose narrow typed contracts.
- Never bypass access controls, permission checks, CAPTCHAs, or sandbox boundaries.

## Batching & Cost Efficiency
- Batch independent file reads and searches in parallel to minimize context bloat.
- Avoid repo-wide full builds when targeted module tests verify the diff.

## Definition of Done
1. Acceptance criteria verified with real command output.
2. Zero leaked credentials or temporary debug logs.
3. Documentation updated when public behavior or CLI flags change.
