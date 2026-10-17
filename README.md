# waterboy firmware releases

Public, **signed** firmware images for waterboy, a plant-watering controller (M5 Atom Lite +
PbHub). The device fetches `manifest-waterboy.json` from the `latest` release, verifies its
ECDSA-P256 signature against public keys built into the firmware, checks the image's SHA-256,
and installs it with health-gated rollback.

The source repo is private; these images contain **no secrets** and are safe to host publicly —
authenticity comes from the signature, not this host.

Each release `vX.Y.Z` holds `waterboy-<ver>.bin`, `manifest-waterboy.json` and
`manifest-waterboy.sig`.
