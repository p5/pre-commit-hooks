# pre-commit-hooks

A collection of useful [pre-commit](https://pre-commit.com/) hooks

## Hooks

### `add-msg-issue-prefix`

A prepare-commit-msg hook for pre-commit.

Extracts the issue identifier from the branch name and prefixes it to the git commit message.

```yaml
-   repo: https://github.com/p5/pre-commit-hooks
    rev: v0.0.5  # Use the release or tag you want to use
    hooks:
    -   id: add-msg-issue-prefix
        args:
            - --template=[{}] # Default --template={} -
```
