# Git and Delivery Workflow

## Branches and commits

- Keep the default branch stable.
- Use short, descriptive branch names such as `feat/user-profile`, `fix/login-timeout`, and `docs/setup-guide`.
- Make focused commits with clear messages, preferably using Conventional Commit prefixes (`feat:`, `fix:`, `docs:`, `refactor:`, `test:`, `chore:`).
- Never commit secrets, local environment files, build artifacts, or unrelated changes.

## Pull requests

A pull request SHOULD include:
- What changed and why.
- How it was tested, with actual commands/results.
- Screenshots or recordings for meaningful UI changes.
- Configuration, migration, or deployment notes.
- Known risks and follow-up work.

Review for correctness, security, accessibility, maintainability, and scope. Resolve review comments before merging.

## Releases and deployment

- Keep deployment steps documented and repeatable.
- Verify environment variables and migrations before release.
- Prefer staged rollout and a rollback or recovery plan for risky changes.
- Monitor relevant logs and health signals after deployment.
- Do not deploy to production without explicit authorization from the project owner.
