# Pull Request Process

See @AGENTS.md for project-wide rules.

## Overview

Workflow for creating and reviewing pull requests.

## Before Creating a PR

1. **Sync dependencies**: `uv sync`
2. **Run tests**: `uv run pytest`
3. **Run linting**: `uv run ruff check .`
4. **Format code**: `uv run ruff format .`

## PR Checklist

- [ ] Tests pass locally
- [ ] Linting passes
- [ ] Code is formatted
- [ ] AGENTS.md updated if patterns learned
- [ ] Relevant docs updated

## Commit Messages

Use conventional commit format:

```
type(scope): description

[optional body]
```

Types:
- `[feature]` - New feature
- `[fix]` - Bug fix
- `[docs]` - Documentation
- `[refactor]` - Code refactoring
- `[test]` - Adding tests
- `[chore]` - Maintenance

## Branch Naming

General pattern
```
type/<github-issue-id>-short-description
```
- github-issue-id: Github issue id for the current changes
- if there is no issue then drop the prefix and use the format: `type/short-description`

Examples:
- `feature/issue-1-user-authentication`
- `fix/issue-2-validation-error`
- `docs/issue-3-api-reference`
- `feature/improve-speed`

