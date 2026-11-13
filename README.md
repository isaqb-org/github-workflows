# github-workflows
Repository contains the GitHub workflows for the various GitHub Actions for curricula

## Releases

A release can be created either by pushing a tag or by creating a release in the GitHub UI.
In both cases the workflow builds the curriculum and attaches the PDFs, the ZIP and the license to the release.

The release text is the content of `CHANGELOG.md`, followed by GitHub's generated release notes.
The generated notes list the changes compared to:

- **Release** (e.g. `2027.1-rev0`): the previous release (e.g. `2025.1-rev2`).
- **First release candidate of a series** (e.g. `2027.1-RC1`): the latest release (e.g. `2025.1-rev2`).
- **Further release candidates** (e.g. `2027.1-RC2`): the previous release candidate of the same series (e.g. `2027.1-RC1`).

- **Release** (`YYYY.N-revN`): text entered in the GitHub UI is replaced.
- **Release candidate** (`YYYY.N-RCN`): text entered in the GitHub UI is kept.
  If no text was entered, the text is built from `CHANGELOG.md` and the generated notes as described above.
