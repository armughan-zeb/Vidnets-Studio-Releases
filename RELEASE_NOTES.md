# Vidnets Studio 1.0.10

Windows x64 release with the latest Vidnets Studio source and bundled runtime.

## Release checks

- Packaged app startup and authentication-denial checks passed.
- The production dependency audit reported no known vulnerabilities.
- The distribution scan reported no secret values or prohibited customer files. It raised two non-blocking warnings for a service-role key *variable name* in packaged auth source; packaged mode disables that fallback.
- A short H.264 Remotion smoke render passed.

The installer is unsigned, so Windows may show an unknown-publisher or SmartScreen notice. This release pass did not run a full long-form generation with live external media and voice providers. Media availability depends on the configured providers and network access.

SHA-256: `3174e90523a6e038b2779c73c742edf097425b3b06bce977fbb0c1ff3b30cbcb`
