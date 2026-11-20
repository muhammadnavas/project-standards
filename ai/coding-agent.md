# Coding Agent Operating Rules

## Before editing
- Inspect repository status and relevant files.
- Identify the existing patterns and tests.
- Check for local instructions and avoid overwriting user changes.
- State assumptions when context is incomplete.

## While editing
- Keep changes minimal and cohesive.
- Reuse existing utilities and components when appropriate.
- Preserve public interfaces unless the task requires a change.
- Do not introduce placeholder implementations or fake data into production paths.
- Do not suppress errors or disable checks to hide failures.
- Do not change unrelated formatting or generated files.

## Before finishing
- Review the diff.
- Run relevant tests and quality checks.
- Verify imports, types, routes, and configuration affected by the change.
- Confirm no secrets, credentials, or personal data were added.
- Summarize what changed and disclose anything not tested.
