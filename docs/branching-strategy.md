# Branching Strategy

## Main Branch

- `main` is the production-ready branch.
- Only stable, reviewed, and tested code should be merged into `main`.
- Tags are often applied on `main` to mark releases.

## Dev Branch

- `dev` is the integration branch for completed feature work.
- It contains code that is ready for testing and staging.
- Teams use `dev` to gather approved changes before releasing.

## Feature Branches

- Create feature branches from `dev`.
- Use descriptive names such as `feature/user-authentication` or `bugfix/fix-login-error`.
- Keep feature branches small and focused.

Example:

```bash
git checkout dev
git pull origin dev
git checkout -b feature/add-readme-content
```

## Git Commits

- Commit early and often.
- Keep each commit atomic and logically grouped.
- Use conventional commit-style messages when possible.

Example commit messages:

- `feat: add branch management documentation`
- `fix: update README section for tags`
- `docs: add setup instructions`

## Merge Workflow

1. Complete work on a `feature/*` branch.
2. Push the branch to the remote repository.
3. Open a pull request targeting `dev`.
4. After review and approval, merge into `dev`.
5. Periodically merge `dev` into `main` for releases.

## Best Practices

- Avoid direct commits to `main`.
- Rebase or merge often to keep branches current with `dev`.
- Use meaningful branch names and commit messages.
- Keep feature branches short-lived.
