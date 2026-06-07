# Setup and Workflow Guide

## Project Setup

1. Clone the repository:

```bash
git clone https://github.com/your-org/git-devops-workflow-demo.git
cd git-devops-workflow-demo
```

2. Confirm the repository structure:

```bash
tree /F
```

3. Review documentation in the `docs/` folder.

## Local Configuration

- Use `.gitignore` to exclude local dependencies and secrets.
- Do not commit `.env` files or generated artifacts.

## How to Create Branches

Use branches to isolate work and keep `main` stable:

```bash
git checkout dev
git pull origin dev
git checkout -b feature/my-new-task
```

Naming conventions:

- `feature/username-description`
- `bugfix/description`
- `hotfix/description`

## How to Commit Code

Make small, atomic commits with descriptive messages:

```bash
git add README.md
git commit -m "docs: add setup and workflow guide"
```

Good commit messages include:
- What changed
- Why it changed
- Any relevant issue or ticket reference

## How to Merge Branches

Merge feature branches into `dev` after review:

```bash
git checkout dev
git pull origin dev
git merge --no-ff feature/my-new-task
git push origin dev
```

Only merge `dev` into `main` when code is ready for production.

## How to Create Tags

Create a release tag after validating `main`:

```bash
git checkout main
git pull origin main
git tag -a v1.0.0 -m "Release version 1.0.0"
git push origin v1.0.0
```

Use semantic versioning and annotated tags for release context.

## How to Create Pull Requests

1. Push your feature branch to the remote repository.
2. Open a pull request against `dev`.
3. Add a clear title and description.
4. Assign reviewers and link related issues.
5. Address review comments and update the branch.

A successful PR should be self-contained and easy to review.
