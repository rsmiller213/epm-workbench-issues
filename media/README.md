# Marketplace listing assets

Screenshots and GIFs for the [Marketplace store page](https://marketplace.visualstudio.com/items?itemName=epmworkbench.epm-workbench).

They live here rather than in the extension repository for one reason: `vsce` rewrites
**relative** links in the packaged `README.md` against the manifest's `repository` field,
which points at this repo. So this is the only place a relative link in the store page can
resolve from — and it keeps multi-megabyte PNGs out of the VSIX.

## Rules

- Reference them from the extension README as `media/<file>` (relative). `vsce` expands
  that to `https://github.com/rsmiller213/epm-workbench-issues/raw/HEAD/media/<file>`.
- `raw/HEAD` means **the store page tracks this branch live** — replacing a file here
  changes the published listing with no extension release. Convenient, and a footgun:
  never delete or rename an asset that a shipped version references.
- Capture on a stock VS Code Dark Modern theme at 2× so the images stay legible when the
  Marketplace scales them down.
- Redact real Pod URLs, customer application names, and member names before committing.
  This repository is public.
