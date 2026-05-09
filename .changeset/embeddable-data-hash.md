---
"@contentauth/c2pa-node": minor
---

Expose `Builder.signDataHashedEmbeddable` and `Builder.signDataHashedEmbeddableAsync`. The Builder produces a signed embeddable manifest from a pre-computed `DataHash` (e.g. raw `SHA-256` of the asset) without requiring the asset bytes at sign time. Useful for sidecar `.c2pa` files and remote-manifest workflows.
