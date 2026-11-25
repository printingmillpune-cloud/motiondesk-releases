# Engineering agent instructions

## Execution and ownership
- Inspect the current repository, scoped instructions, existing tests, deployment configuration and open issues before editing. Preserve existing requirements; do not invent project state or replace existing architecture without approval.
- Turn the request into acceptance criteria and identify dependencies, risks, next steps and independent work. Use separate worktrees/branches for parallel changes; avoid overlapping edits. Use separate developer and reviewer/tester sessions when the environment supports it.
- Prefer small, reviewable PRs. Never bypass required checks, branch protections, permissions or existing release approvals. Do not change production, secrets, billing or customer data without the appropriate authorization.
- For ordinary failures, attempt up to two distinct justified corrections, then report exact error and reproduction steps; continue independent work.
- Before marking complete, report commit/PR, actual commands and results, skipped checks, environment, remaining blockers and rollback approach. Never call a feature verified from code inspection alone.
- Maintain a repository-local status/roadmap/known-issues record; distinguish confirmed facts, hypotheses and pending work. Never claim agents are running when no session is active.

## Review and release gates
- A separate reviewer should inspect the final diff against acceptance criteria, prioritizing correctness, regression, security, privacy, data integrity and compatibility. Report actionable findings with file and line references. Resolve blocking findings and rerun relevant checks on the final revision.
- Run existing lint/type/build/unit/integration/browser tests as appropriate. Record exact results; skipped tests are not passes. Use isolated test data and environments; never use production customer data as fixtures.
- Review and test the final commit before release. Verify the deployed version and relevant live functionality using safe checks; preserve a rollback path.
- Never expose credentials, tokens, customer records, private project files or production logs in commits, PRs, screenshots or public reports.

## Release distribution rules
- This is a public release-distribution repository, not evidence of access to the desktop app source. Follow README.md.
- Never upload customer videos, exports, credentials, API keys, project settings or local projects. Only verified code-only updates belong in releases.
- Flag any latest.json update without a matching existing release ZIP and a verified SHA-256. Do not publish a new release or change latest.json for documentation work.
