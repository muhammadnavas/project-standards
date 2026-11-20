# Project Standards

A shared, practical baseline for planning, designing, building, reviewing, and maintaining software projects.

These standards are intended to be reused across personal, academic, and production projects. They are deliberately technology-agnostic: each project may choose its own stack, but should document its decisions and follow the applicable quality and safety rules.

## How to use this repository

1. Read this README and the applicable standards before starting a project.
2. Copy or reference the relevant files in the project repository.
3. Add an `AGENTS.md` (or equivalent agent instruction file) that points coding agents to these standards.
4. Create a project brief documenting goals, users, scope, stack, architecture, risks, and acceptance criteria.
5. Record deviations from these standards and explain why they are justified.

## Standards hierarchy

- **MUST**: required unless a documented exception is approved.
- **SHOULD**: recommended; deviations need a practical reason.
- **MAY**: optional guidance.

Project-specific requirements and applicable laws take precedence where they are stricter. Security, privacy, and accessibility requirements must not be weakened for convenience.

## Contents

- [Brand and UI standards](docs/branding.md)
- [Engineering standards](docs/engineering.md)
- [Architecture standards](docs/architecture.md)
- [System requirements and quality attributes](docs/system-requirements.md)
- [Security and privacy](docs/security-privacy.md)
- [AI and coding-agent instructions](ai/README.md)
- [Git and delivery workflow](docs/workflow.md)
- [Project brief template](templates/project-brief.md)
- [Agent entry-point instructions](AGENTS.md)

## Project-specific configuration

Every project MUST define:
- Purpose, target users, and success criteria.
- Supported platforms and accessibility expectations.
- Technology stack and versions.
- Architecture and data-flow overview.
- Environment variables and external dependencies (never their secret values).
- Local setup, test, build, and deployment instructions.
- Known limitations, risks, and operational ownership.

Do not blindly copy every recommendation. Select what applies, keep the project simple, and document important decisions.

## Maintenance

Treat these documents as living standards. Propose changes through pull requests, explain the reason and impact, and avoid introducing rules that cannot be consistently followed.
