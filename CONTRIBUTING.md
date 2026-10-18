# Contributing to cur8d

Thank you for your interest in contributing to **cur8d**! Our goal is to provide opinionated, production-ready project templates and tooling for modern developers.

## Code of Conduct

All contributors and participants agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md).

## Getting Started

1. **Fork and Clone**: Fork the target repository and clone it locally.
2. **Tools & Dependencies**: We use [`mise`](https://mise.jdx.dev) to manage runtimes and project tasks.

   ```bash
   mise install
   mise run dev
   ```

3. **Branching**: Create a feature branch off `main`:

   ```bash
   git checkout -b feat/your-feature-name
   ```

## Development Workflow & Tasks

Every repository in the cur8d ecosystem standardizes commands with `mise`:

| Command           | Description                                       |
| :---------------- | :------------------------------------------------ |
| `mise run dev`    | Set up local development environment              |
| `mise run lint`   | Run code quality linters and format checks        |
| `mise run format` | Auto-format codebase                              |
| `mise run test`   | Run test suite with coverage                      |
| `mise run verify` | Full verification (lint, typecheck, format, test) |

Always ensure `mise run verify` passes before submitting your changes.

## Conventional Commits

We follow [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` New features or additions
- `fix:` Bug fixes
- `docs:` Documentation updates
- `style:` Formatting or whitespace changes
- `refactor:` Code refactoring without behavior change
- `perf:` Performance improvements
- `test:` Adding or updating tests
- `chore:` Dependency updates, tooling, and workflow maintenance

## Submitting Pull Requests

1. Keep commits atomic and self-contained (one logical change per commit).
2. Follow the repository's [Pull Request Template](.github/PULL_REQUEST_TEMPLATE.md).
3. Ensure all automated tests and linter checks pass (`mise run verify`).
4. Rebase against `main` before requesting review (`git pull --rebase origin main`).
