# EPM Workbench — Issues

Public issue tracker for **[EPM Workbench for VS Code](https://marketplace.visualstudio.com/items?itemName=epmworkbench.epm-workbench)**, a
VS Code-native IDE for Oracle EPM calculation development.

**There is no source code here.** The extension is closed source; this repository exists
so that everyone who installs it has a public, searchable place to report bugs and request
features without needing an account on anything but GitHub.

## Report something

| I want to… | Go here |
| --- | --- |
| Report a bug | [New bug report](https://github.com/rsmiller213/epm-workbench-issues/issues/new?template=bug_report.yml) |
| Request a feature | [New feature request](https://github.com/rsmiller213/epm-workbench-issues/issues/new?template=feature_request.yml) |
| Report a security vulnerability | **Do not open an issue** — see [SECURITY.md](SECURITY.md) |
| Ask a billing / Seat Key question | <billing@epmworkbench.com> |
| Read the docs | <https://epmworkbench.com/docs/getting-started/install> |

Search [existing issues](https://github.com/rsmiller213/epm-workbench-issues/issues?q=is%3Aissue)
before filing — a duplicate is slower to resolve than a comment on the original.

## What to expect

- Issues are triaged, labelled, and closed here; the fix itself lands in the private
  extension repository and ships in a numbered release.
- Releases and their notes: <https://marketplace.visualstudio.com/items/epmworkbench.epm-workbench/changelog>
- Never paste Oracle credentials, Seat Keys, Pod URLs, or customer member names into an
  issue. This tracker is public and indexed. Redact before you post; see
  [SECURITY.md](SECURITY.md) if you already posted something sensitive.

## `media/` — Marketplace listing assets

The extension manifest sets `repository` to this repo, which means **relative image links
in the Marketplace store page resolve against it**. Screenshots and GIFs used in the
listing therefore live in [`media/`](media/) and are referenced from the extension README
as `media/<file>`. See [`media/README.md`](media/README.md) for the URL rules.
