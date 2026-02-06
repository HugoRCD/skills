# Create Commit Name

Suggest a conventional commit message name for the current changes.

## Purpose

This skill analyzes the current code changes and suggests a commit message that follows the conventional commit convention: `type(scope): title`.

## Conventional Commit Format

The format is: `type(scope): title`

### Types

- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation only changes
- **style**: Changes that don't affect code behavior (formatting, whitespace, missing semi-colons, etc)
- **refactor**: Code change that neither fixes a bug nor adds a feature
- **perf**: A code change that improves performance
- **test**: Adding missing tests or correcting existing tests
- **build**: Changes that affect the build system or external dependencies
- **ci**: Changes to CI configuration files and scripts
- **chore**: Other changes that don't modify src or test files
- **revert**: Reverts a previous commit

### Scope (optional)

The scope should be the name of the affected component, module, or area (e.g., `api`, `ui`, `auth`, `database`).

### Title

A short, imperative description of the change:
- Use lowercase
- No period at the end
- Keep it under 72 characters
- Start with a verb (e.g., "add", "update", "remove", "fix")

## Workflow

1. Analyze the git diff or staged changes
2. Identify the type of change (feat, fix, docs, etc.)
3. Determine the scope (component or area affected)
4. Write a concise, descriptive title in imperative mood
5. Suggest ONE commit message in the format: `type(scope): title`

## Examples

Good commit messages:
- `feat(auth): add oauth2 login support`
- `fix(api): resolve null pointer exception in user endpoint`
- `docs(readme): update installation instructions`
- `refactor(database): simplify query builder logic`
- `test(auth): add unit tests for login validation`
- `chore(deps): upgrade dependencies to latest versions`
- `style(ui): format code with prettier`

Bad commit messages:
- `Update files` (not specific, missing type)
- `feat: Add Feature` (not lowercase, too vague)
- `fixed bug` (missing scope, past tense)
- `WIP` (not descriptive)

## Output Format

Provide the suggested commit message in a markdown code block:

```
type(scope): title
```

Provide only ONE suggestion - the best fit for the changes.
