# CLAUDE.md

## Project Overview

This repository contains a sample Node.js web application used for demonstrating development workflows, Git operations, CI/CD pipelines, testing, and documentation practices.

## Technology Stack

* Node.js
* Express.js
* Jest
* Docker
* GitHub Actions

## Development Standards

### Code Style

* Use ES6+ syntax.
* Prefer `const` over `let` whenever possible.
* Use async/await instead of promise chains.
* Keep functions under 50 lines when practical.
* Add comments only when business logic is not obvious.

### File Organization

* Routes belong in `src/routes/`
* Controllers belong in `src/controllers/`
* Business logic belongs in `src/services/`
* Utility functions belong in `src/utils/`
* Middleware belongs in `src/middleware/`

### Testing

When modifying code:

1. Update or create relevant unit tests.
2. Ensure existing tests continue to pass.
3. Add integration tests for new API endpoints.

### Documentation

Update documentation when:

* Adding new API endpoints
* Changing configuration settings
* Modifying deployment procedures

Relevant documentation files:

* docs/api.md
* docs/architecture.md
* docs/deployment.md

### Git Commit Guidelines

Use conventional commit messages:

* feat: add new functionality
* fix: resolve bug
* docs: update documentation
* test: add or update tests
* refactor: improve code structure
* chore: maintenance tasks

Examples:

feat: add product search endpoint
fix: handle missing user email validation

### Pull Request Requirements

Before creating a PR:

* Run tests
* Update documentation if necessary
* Ensure linting passes
* Verify Docker build succeeds

### Security

* Never commit secrets.
* Never commit API keys.
* Use environment variables for credentials.
* Sanitize all user input.

### Docker

When changing dependencies:

* Update Dockerfile if required.
* Verify docker-compose.yml remains functional.

### Preferred Response Format

When making changes:

1. Explain the goal.
2. List files modified.
3. Summarize changes.
4. Mention potential risks.
5. Suggest next steps.
