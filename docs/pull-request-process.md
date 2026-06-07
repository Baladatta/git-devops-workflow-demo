# Pull Request Process

## Purpose of Pull Requests

Pull requests provide a formal review process, capture discussion, and give the team an opportunity to verify changes before merging.

## Pull Request Workflow

1. Finish your work on a `feature/*` branch.
2. Push the branch to the remote repository.
3. Open a pull request against `dev`.
4. Include a clear summary and list of changes.
5. Reference related issues or tickets.
6. Request at least one review from a teammate.
7. Respond to feedback and update the branch.
8. Merge only after approval and verification.

## Review Checklist

- Does the branch follow the project's branch naming conventions?
- Are commit messages descriptive and grouped logically?
- Is the code complete and tested?
- Are there any unnecessary files or debug artifacts?
- Does the PR description explain the goal and impact?

## Merge Options

- `Merge commit` preserves full history.
- `Squash merge` creates a single commit for a clean history.
- `Rebase and merge` can keep a linear history while preserving changes.

Choose the merge style that fits your team policy.

## Post-Merge Steps

1. Delete the merged feature branch from the remote repository.
2. Pull the latest `dev` changes locally.
3. If `dev` is ready, open a PR from `dev` to `main`.
4. Tag releases after merging into `main`.
