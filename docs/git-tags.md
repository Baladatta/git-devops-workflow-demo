# Git Tags

## What Are Git Tags?

Git tags mark specific commits as important points in history, such as releases or versioned milestones.

## Tag Types

- Annotated tags (`-a`) store metadata, a message, and the tagger information.
- Lightweight tags are simpler references with no extra metadata.

## Recommended Usage

- Use annotated tags for releases:

```bash
git checkout main
git pull origin main
git tag -a v1.0.0 -m "Release v1.0.0"
git push origin v1.0.0
```

- Use tag names that follow semantic versioning:
  - `v1.0.0`
  - `v1.1.0`
  - `v1.1.1`

## Viewing Tags

```bash
git tag
```

To see tag details:

```bash
git show v1.0.0
```

## Best Practices

- Tag on the `main` branch after final approval.
- Keep tags stable and only update version numbers for new releases.
- Link tags to release notes or changelogs when possible.

## Example Workflow

1. Merge approved changes into `main`.
2. Tag the current commit.
3. Push the tag to the remote repository.

This makes it easy to track release history and rollback if needed.
