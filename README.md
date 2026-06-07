# git-devops-workflow-demo

## Project Overview

This repository is a DevOps internship demo that showcases professional Git version control best practices. It illustrates how to structure branches, create commits, manage pull requests, apply tags, and maintain documentation for a reproducible workflow.

## Objective

- Demonstrate how to use Git and GitHub effectively in a team environment.
- Explain branch usage and repository organization.
- Document pull request and merge workflows.
- Show how tags support release management.

## Tools Used

- Git
- GitHub or Git-compatible hosting service
- Markdown for documentation
- `.gitignore` to keep repository clean

## Git Workflow Explanation

This project uses a branching workflow with separate branches for production-ready code, active development, and feature work. The workflow supports collaboration, code review, and stable releases.

## Branching Strategy

- `main` - Production-ready branch. Always stable and deployable.
- `dev` - Integration branch for completed features and release preparation.
- `feature/*` - Branches for individual tasks, bug fixes, or experiments.

Read full details in `docs/branching-strategy.md`.

## Pull Request Workflow

1. Create a `feature/*` branch from `dev`.
2. Work on the feature with frequent, descriptive commits.
3. Push the branch to the remote repository.
4. Open a pull request against `dev`.
5. Request review, address comments, and update the branch.
6. Merge once the PR is approved and tests pass.

Detailed guidance is available in `docs/pull-request-process.md`.

## Merge Strategy

- Merge `feature/*` branches into `dev` using a merge commit or squash merge.
- Only merge `dev` into `main` after validation and approval.
- Use fast-forward or merge commits depending on team policy.
- Keep history readable by avoiding direct commits to `main`.

## Git Tags

Tags are used to mark important releases and milestones. Use annotated tags for release notes and light-weight tags for temporary checkpoints.

Learn more in `docs/git-tags.md`.

## .gitignore Usage

The `.gitignore` file prevents build artifacts, environment files, dependencies, and logs from being committed. This keeps the repository clean and secure.

Ignored paths:
- `node_modules/`
- `.env`
- `*.log`
- `dist/`
- `build/`

## Screenshots Section

This repository includes a `screenshots/` folder for UI examples of workflows, diagrams, or GitHub PR visuals. Populate this folder with images illustrating your process.

## Conclusion

This project is a reference for DevOps interns learning Git best practices. It emphasizes branch discipline, clear commits, documented workflows, and consistent repository hygiene.

## Documentation

- `docs/setup.md` - Setup and workflow quick starts.
- `docs/branching-strategy.md` - Branch definitions and feature branch examples.
- `docs/pull-request-process.md` - PR steps, review expectations, and merge guidance.
- `docs/git-tags.md` - Tag creation, usage, and versioning recommendations.
