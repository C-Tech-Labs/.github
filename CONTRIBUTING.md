# Contributing to C-Tech-Labs

Thank you for investing time to improve C-Tech-Labs projects. This guide outlines expectations for quality, security, and collaboration so we can ship dependable software together.

## Getting started
- Fork the repository and clone it locally.
- Install project prerequisites (language runtimes, package managers, linters) as documented in the project README.
- Create a focused branch from `main`, e.g., `feat/<short-description>` or `fix/<issue-id>`.

## Development workflow
1. **Design first:** For non-trivial changes, open an issue or draft PR describing the problem, scope, and approach. Include success metrics and rollback considerations.
2. **Small, atomic commits:** Use [Conventional Commits](https://www.conventionalcommits.org/) for clarity (e.g., `feat: add audit logging`). Each commit should pass tests.
3. **Testing and quality:**
   - Run unit, integration, and lint checks relevant to the stack.
   - Add or update tests to cover new behavior and regression cases.
   - Keep coverage steady or improving; highlight any intentional gaps.
4. **Security:**
   - Prefer least-privilege defaults and secure-by-default configs.
   - Avoid introducing secrets into code or history; use secret scanners if available.
   - Document threat considerations and mitigations for sensitive changes.
5. **Documentation:** Update README, changelogs, and inline docs so future contributors understand intent and usage.

## Pull requests
- Link related issues in the PR description (`Fixes #123`).
- Provide a concise summary, testing evidence (commands, screenshots), and a rollback plan in the template.
- Mark the PR as **Draft** until all required checks pass.
- Request reviews from relevant owners; pair on risky changes when possible.
- Address feedback promptly; follow up with additional tests if fixes are made.

## Code style
- Honor linters and formatters configured for the repository.
- Prefer clear, maintainable solutions over cleverness; optimize only with data.
- Keep functions cohesive and small; document non-obvious behavior and edge cases.

## Release management
- Follow semantic versioning where applicable.
- Include migration guides and operational notes for changes that impact deployments.
- Backport fixes to supported release lines when required; coordinate with the release manager.

## Reporting issues
If you find a bug or have a feature request, please [open an issue](../../issues/new/choose) and provide:

- **Summary:** What is happening and why it matters.
- **Expected vs. actual behavior** with screenshots or logs when possible.
- **Steps to reproduce:** Minimal, reliable reproduction steps.
- **Environment:** OS, runtime versions, and configuration that might be relevant.

Before opening a new issue, search existing issues and discussions to avoid duplicates.

## Licensing
By contributing, you agree your contributions are licensed under the MIT license unless otherwise noted.
