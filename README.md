# Vidnets Studio Releases

This repository is the stable update channel for Vidnets Studio.

- `latest.json` is fetched by the desktop app and contains the current version,
  installer URL, size, and SHA-256 checksum.
- `RELEASE_NOTES.md` and `checksums.txt` are human-reviewable release records.
- The Windows installer is uploaded to the matching GitHub Release (`vX.Y.Z-build.<build-id>`)
  as an asset; it is intentionally not committed to git.

Prepare metadata from the application repository with:

```text
npm run release:prepare
```

Then commit the metadata in this folder and upload the staged EXE as the
matching GitHub Release asset. The desktop app only downloads HTTPS GitHub
assets whose filename, size, and SHA-256 match `latest.json`.

Releases use distinct build tags so previous installers remain available. Publish the new asset and verify its GitHub digest before pushing the update-channel manifest.

The current installer is also linked at https://vidnets.com/releases.html.
Lifetime Pro is available at https://vidnets.com/#pricing for the one-time $149 launch offer.
Downloading the installer does not grant access; use the account associated with a paid purchase.
