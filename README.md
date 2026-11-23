# Kinto update feed

The Kinto launcher app reads `latest.json` in this repo to check for updates
and downloads the package named there. The package travels base64-encoded
(`.apk.b64`) because GitHub file pushes are text-only; the app decodes it and
verifies the SHA-256 hash and signing identity before installing.

This repo contains only the update feed and app packages - no source code.
The Kinto source lives in the private `kinto` repo.
