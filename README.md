# MotionDesk – update releases

This public repository distributes **code-only updates** to the MotionDesk desktop app.

- Never upload customer videos, exports, credentials, API keys, or project settings.
- A verified code-only ZIP is stored at `releases/MotionDesk_Update_vX.Y.Z.zip`.
- The app reads `latest.json` to discover updates. Each release is checked with SHA-256 before installation.
- Existing local projects and data are not included in release packages.

Initial release candidate: **v0.3.6** (music mixer, preview approval, Windows video-render fixes).

**Safety:** `latest.json` must not be published until its referenced ZIP is present at the correct path.