# Vidnets Studio Releases

This repository is the stable update channel for Vidzeo Studio.

- `latest.json` is fetched by the desktop app and contains the current version,
  installer URL, size, and SHA-256 checksum.
- `RELEASE_NOTES.md` and `checksums.txt` are human-reviewable release records.
- The Windows installer is uploaded to the matching GitHub Release (`vX.Y.Z`)
  as an asset; it is intentionally not committed to git.

Prepare metadata from the application repository with:

```text
npm run release:prepare
```

Then commit the metadata in this folder and upload the staged EXE as the
matching GitHub Release asset. The desktop app only downloads HTTPS GitHub
assets whose filename, size, and SHA-256 match `latest.json`.
