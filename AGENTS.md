# Repository Guidelines

## Project Structure & Module Organization

This repository currently has no application source, tests, assets, or package manifest. Add new code under `src/`, automated tests under `tests/`, and static files under `assets/` when those directories become necessary. Keep related modules and their tests easy to locate by using matching names, such as `src/timer.js` and `tests/timer.test.js`. The existing `.agents/`, `.codex/`, and `.aws/` directories are empty workspace directories, not application modules.

## Build, Test, and Development Commands

No build system, test runner, or local server is configured yet, so there are no working project commands to list. When adding a runtime or toolchain, document its setup and exact commands in a `README.md` and define reproducible scripts in the relevant manifest (for example, `package.json`). Verify those commands from a clean checkout before describing them as supported.

## Coding Style & Naming Conventions

Follow the formatter and linter selected with the first implementation. Commit their configuration so contributors get the same results. Until then, use consistent indentation within each file, descriptive module names, and names that reveal purpose. Prefer small modules with clear inputs and outputs. Do not introduce a second naming or formatting style without a project-wide reason.

## Testing Guidelines

There is no test framework or coverage target yet. Add tests alongside the first behavior they protect and document how to run them. Name tests after the behavior or module under test, and cover normal operation plus important failure or boundary cases. Avoid claiming coverage percentages until a coverage tool is configured.

## Commit & Pull Request Guidelines

No Git history is available here, so no existing commit-message convention can be inferred. Use short, imperative subjects that describe the change, such as `Add timer pause control`. Keep pull requests focused; include a summary, how the change was verified, and links to related issues when applicable. Include screenshots or a short recording for visible interface changes.

## Security & Configuration

Do not commit credentials, local environment files, or contents of `.aws/`. Document required configuration with safe example values once the application needs it.
