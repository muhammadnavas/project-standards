# System Requirements and Quality Attributes

Every project MUST define requirements appropriate to its scope. Avoid inventing numerical targets without measuring or agreeing on them.

## Functional requirements

Describe what the system must do from the user's or integrating system's perspective. Requirements SHOULD be specific, testable, and prioritized.

## Non-functional requirements

Consider and document:

- **Performance:** expected workload, response-time goals, resource limits, and measurement method.
- **Reliability:** availability expectations, failure modes, recovery, backups, and data-loss tolerance.
- **Security:** authentication, authorization, secrets, input validation, and threat assumptions.
- **Privacy:** data collected, purpose, retention, deletion, and third-party sharing.
- **Accessibility:** supported assistive technology and accessibility target.
- **Compatibility:** browsers, devices, operating systems, runtimes, and supported versions.
- **Scalability:** expected growth and known bottlenecks; scale only when evidence requires it.
- **Maintainability:** code ownership, documentation, test strategy, and upgrade approach.
- **Observability:** logs, metrics, traces, alerts, and health checks as appropriate.

## Environments

Separate local, test/staging, and production configuration. Production data and credentials MUST NOT be copied into local development or test environments unless explicitly authorized and safely sanitized.

## Definition of done

A feature is complete when:
- Acceptance criteria are met.
- Relevant tests pass.
- Lint/type checks/build pass where configured.
- Security and accessibility implications are considered.
- Documentation and configuration examples are updated.
- No secrets or unintended generated files are committed.
- Known limitations are recorded.
