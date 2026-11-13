# github-workflows
Repository contains the GitHub workflows for the various GitHub Actions for curricula

## Releases

A release can be created either by pushing a tag or by creating a release in the GitHub UI.
In both cases the workflow builds the curriculum and attaches the PDFs, the ZIP and the license to the release.

- **Release** (`YYYY.N-revN`): the release text is always taken from `CHANGELOG.md`.
  Text entered in the GitHub UI is replaced.
- **Release candidate** (`YYYY.N-RCN`): text entered in the GitHub UI is kept.
  If the release candidate is created by pushing a tag, the text is taken from `CHANGELOG.md`.
