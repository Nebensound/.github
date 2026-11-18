# .github

What GitHub inherits across the Nebensound organization: issue forms, the pull
request template, community health files and workflow templates.

GitHub reads a public repository named `.github` and applies its community
files to every repository of the organization that does not bring its own. The
files themselves arrive with later changes; this repository first states what
it is for and what belongs in it.

## What belongs here

Only what GitHub inherits from a repository of this name, plus this
repository's own housekeeping files:

- issue forms and the pull request template,
- community health files such as the code of conduct, the contributing guide
  and the security policy,
- the funding file,
- workflow templates.

## What does not belong here

- Secrets, tokens or credentials.
- Internal host names or anything else that is not meant to be public.
- Proprietary code.
- Callable workflows. They live in the pipeline repository, and every
  repository calls them from there.

The repository has to stay public, because GitHub does not perform the
inheritance otherwise. Everything in it, including its history, is readable by
anyone.

## How inheritance behaves

1. **A local file of the same kind wins.** A repository that has its own file,
   for example a `SECURITY.md`, uses that one and ignores the inherited file.
2. **Issue forms are not merged.** A repository with its own `ISSUE_TEMPLATE`
   folder replaces the inherited set as a whole, so it has to bring the full
   set it wants to offer.
3. **Inherited files appear in no clone.** They exist only on GitHub and show
   up in the web interface. A file that has to be in the working tree, for
   example for a local check, must be committed to that repository itself.

## Licence

[EUPL-1.2](LICENSE).
