# Instructions for AI Coding Agents

Before making changes in a project that adopts this standards repository:

1. Read the project's own README, architecture notes, and local agent instructions.
2. Read the relevant standards in this repository. Start with `README.md`; then consult engineering, architecture, security, branding, workflow, and AI guidance as applicable.
3. Treat the existing codebase as the source of truth. Inspect before editing; do not assume a greenfield project.
4. Preserve established conventions unless they are unsafe or clearly broken. Explain meaningful deviations.
5. Make the smallest coherent change that solves the requested problem. Avoid unrelated refactors and unnecessary dependencies.
6. Never expose, log, commit, or fabricate secrets. Do not run destructive commands or deploy changes without explicit authorization.
7. Add or update tests for changed behavior. Run relevant tests, lint, type checks, and builds where available.
8. Report what changed, files affected, checks run, results, and any remaining risks.

## Implementation expectations

- Prefer clear, maintainable, typed code where the language supports it.
- Validate untrusted input at system boundaries.
- Handle errors explicitly; do not silently swallow failures.
- Keep secrets and environment-specific configuration outside source control.
- Follow the project's existing design system and accessibility patterns.
- Do not claim a test, build, deployment, or verification succeeded unless it actually ran and passed.

If project instructions conflict with these shared standards, follow stricter security and legal requirements, then the project's explicit requirements. Call out unresolved conflicts instead of guessing.
