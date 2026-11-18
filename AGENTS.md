# Contribution Rules

This repository holds what GitHub inherits across the Nebensound organization:
issue forms, the pull request template, community health files and workflow
templates. It is public, so everything in it, including its history, is
readable by anyone. These rules apply to every change, whoever or whatever
writes it.

## What belongs here

- Only files that GitHub inherits from a repository named `.github`. Anything
  else belongs in the repository it concerns.
- Callable workflows do not live here. They live in the central pipeline
  repository.
- Keep the inherited files generic. A repository that needs something specific
  brings its own file, which wins over the inherited one.
- Issue forms are not merged: a repository with its own `ISSUE_TEMPLATE` folder
  has to bring the full set. Keep that in mind when changing a form.

## Nothing private

- No secrets, tokens or credentials.
- No private repository, internal host name or internal document is named,
  linked or quoted: not in files, commit messages, issues, pull requests or
  comments.
- No proprietary code.

## Language and content

- Everything is English: documentation, comments, commit messages, issues and
  pull requests.
- Commit messages follow Conventional Commits.

## Checks

- Markdown is formatted with Prettier and linted with markdownlint, YAML with
  yamllint, TOML with Taplo.
- Until the repository calls the central pipeline, the pull request states the
  local results of these checks and names every check that could not be run
  with its reason.
