# Security and Privacy Standards

Security is a baseline requirement, not a final polishing step.

- Store secrets in a trusted secret manager or deployment environment; never commit them.
- Commit only sanitized environment examples such as `.env.example`.
- Enforce authorization on the server for protected operations; hiding UI controls is not access control.
- Apply least privilege to users, services, tokens, and database accounts.
- Validate and normalize untrusted input; use parameterized database queries and safe output encoding.
- Use secure, supported authentication and session mechanisms.
- Protect against common web risks such as injection, XSS, CSRF, SSRF, insecure direct object references, and unsafe file uploads where relevant.
- Use HTTPS in deployed environments.
- Avoid exposing stack traces, secrets, internal IDs, or sensitive data in client-facing errors.
- Minimize personal data collection and define retention and deletion behavior.
- Redact sensitive values from logs, analytics, screenshots, and support artifacts.
- Keep dependencies and runtimes patched; review security advisories.
- Back up important data and periodically verify that restoration works.

For a suspected incident: contain the exposure, rotate affected credentials, preserve relevant evidence, assess impact, and follow applicable notification and response obligations. Never paste live credentials into AI tools or issue trackers.
