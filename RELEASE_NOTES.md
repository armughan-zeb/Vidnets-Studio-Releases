# Vidnets Studio 1.0.8

Windows x64 security and runtime update. Earlier installer releases were withdrawn; install the current build from this official release page.

## Changes

- Removed administrative web tools, session secrets, and development-only files from the customer package.
- Export usage settlement now requires a signed-in owner and verifies that the export belongs to that account.
- Packaged builds no longer load private developer `.env` settings or enable local developer authentication.
- Restricted desktop commands to the trusted app frame and blocked arbitrary local-file navigation.
- Updated the bundled Python, Node.js, Electron, and Remotion browser runtimes.

## Verification

- 87 regression tests plus 4 subtests passed; 4 desktop security tests passed.
- Packaged backend checks confirmed that admin routes are unavailable and unsigned generation requests are rejected.
- A packaged 18-frame Remotion render passed H.264 probing. Review generated videos for source accuracy and media availability before publishing.

## Installation note

This installer is unsigned. Windows may show an unknown-publisher or SmartScreen notice.

SHA-256: `ff555a25ac2718e0cff821708ace18897b07452d599d6338645177595b49690b`
