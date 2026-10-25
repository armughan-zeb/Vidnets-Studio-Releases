# Vidnets Studio 1.0.6

Windows maintenance release focused on media contract integrity, YouTube footage downloading, UI progress clarity, and grounded motion graphic fallbacks.

## Fixed

- **Grounded Motion Graphic Fallbacks Enabled**: Grounded graphics fallback is now fully enabled and accepted across the pipeline without being misclassified as rejected emergency media.
- **Organization & League Subject Typing**: Sports leagues (NFL, NBA, MLB, FIFA, etc.), organizations, and franchises are now properly classified as organizational entities rather than individual human persons, eliminating false strict facial-identity rejection on sports and documentary B-roll.
- **YouTube High-Risk Channel Over-Blocking Resolved**: Fixed overly broad uppercase acronym veto that inadvertently blocked official sports league and entertainment channels (such as NFL, NBA, UFC, F1, IGN).
- **YouTube Format Fallback**: Added progressive and 480p format fallbacks in yt-dlp so videos without separate high-bitrate adaptive 720p+ streams no longer abort with format unavailable errors.
- **Interactive UI Progress & Queue Overlay**: When a job pauses or requires action, the overlay clearly reports "Action needed" with the specific status and provides a one-click "Retry Video" button, eliminating confusing "Please wait / Preparing media" freezes.

## Verified

- 32 Python regression tests passing, including tests for grounded graphic policies, organizational typing, format recovery, and queue reliability.
- Full end-to-end documentary packaging and Remotion motion graphics verification.
- Offline bundled runtime: Node.js, Python, FFmpeg, and Remotion headless browser.

SHA-256: `38788e5ef86e7b5ed4314f047cba3ffad99491586e0d13bc82f859647f160efa`
