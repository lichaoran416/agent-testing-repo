# agent-testing-repo

A small test repository used to try out and demonstrate the dsh-superagent
workflow end to end: a request arrives from a chat thread, an agent picks it
up, makes a focused change on a branch, and opens a pull request for review.

## Purpose

This repository is intentionally tiny. It exists so that the whole automation
path can be exercised without worrying about build tooling or large codebases:

- receiving a request from a chat thread (Feishu) or a GitHub issue;
- creating a dedicated branch and making a small, reviewable change;
- opening a pull request with a clear description;
- letting CI, reviewers, and the delivery step run against it.

## Contents

| Path        | Description                   |
| ----------- | ----------------------------- |
| `README.md` | Project overview (this file). |

## Getting started

There is nothing to build or install — the repository has no dependencies and
no build step.

```bash
git clone https://github.com/lichaoran416/agent-testing-repo.git
cd agent-testing-repo
```

## Contributing

1. Create a branch: `git switch -c my-change`
2. Make the change and commit it.
3. Push the branch and open a pull request against `main`.

Changes made by the automation agent are delivered as pull requests, so every
change can be reviewed before it lands on `main`.

## License

No license is declared; this repository is for testing and demonstration only.
