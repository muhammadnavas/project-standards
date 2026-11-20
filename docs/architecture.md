# Architecture Standards

## Design approach

Choose architecture based on project size, team needs, expected change, and operational constraints. Do not introduce microservices, event buses, queues, or complex abstractions without a demonstrated need.

## Boundaries

- Separate presentation, business/domain logic, and infrastructure concerns where useful.
- Keep business rules out of UI components and transport handlers.
- Define clear interfaces between modules and external services.
- Avoid circular dependencies and hidden shared mutable state.
- Keep modules cohesive and expose small, intentional public interfaces.

## APIs and data

- Define request/response contracts and validate them at boundaries.
- Use consistent naming, status codes, pagination, filtering, and error formats.
- Version public APIs when breaking changes are unavoidable.
- Use database constraints and transactions to protect data integrity.
- Design migrations to be reviewable and safe to apply; consider rollback or forward-recovery.
- Avoid returning internal implementation details or sensitive fields.

## Reliability and operations

- Set sensible timeouts for network calls.
- Use bounded retries with backoff only for transient failures; avoid retrying non-idempotent operations blindly.
- Make operations idempotent where practical.
- Add structured logs and health checks appropriate to the deployment.
- Avoid logging credentials, tokens, personal data, or full sensitive payloads.
- Document external dependencies and failure behavior.

## Architecture decisions

For meaningful decisions, record context, options considered, decision, consequences, and date in a short ADR (Architecture Decision Record). Keep diagrams aligned with the implementation.
