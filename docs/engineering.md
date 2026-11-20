# Engineering Standards

## General principles

- Prefer simple, readable, maintainable solutions over clever or premature abstractions.
- Follow the language and framework conventions already established in the project.
- Use descriptive names and small, cohesive functions/modules.
- Keep responsibilities clear; avoid unnecessary coupling and duplicated logic.
- Do not add dependencies for functionality that is trivial to implement safely.
- Keep configuration separate from application logic.

## Code quality

- Use the formatter, linter, and type checker configured by the project.
- Add types or schemas at important boundaries.
- Validate external input; do not trust browser, user, file, or API data.
- Handle expected failures explicitly and provide actionable error messages.
- Avoid empty catch blocks, unexplained magic values, dead code, and commented-out code.
- Keep functions focused and avoid deeply nested control flow.
- Add comments to explain intent or non-obvious constraints, not to narrate obvious code.

## Testing

- Add tests for new behavior and bug fixes.
- Cover normal cases, edge cases, invalid input, and failure paths.
- Prefer deterministic tests; isolate network, time, randomness, and external services.
- Test behavior rather than implementation details.
- Do not delete or weaken tests merely to make a build pass.

## Dependencies

- Prefer maintained, reputable packages.
- Review license, maintenance activity, security advisories, and package scope before adoption.
- Pin or lock dependencies using the ecosystem's standard lockfile.
- Remove unused dependencies and keep upgrades deliberate.

## Documentation

- Document setup, configuration, scripts, architecture, and important trade-offs.
- Keep README instructions accurate and runnable.
- Document public APIs and non-obvious behavior.
- Update documentation when behavior or configuration changes.

## Pull request readiness

A change SHOULD be focused, tested, documented where needed, and reviewed for security, accessibility, performance, and backward compatibility.
