---
status: active
last_touched: 2026-07-18
deploy: git push origin main --tags
---

# Mono Voice

Distribution repository for the `mono-voice` Schwung sound generator. The
canonical source and ARM build remain in `../mono`; this project gives Schwung
Manager a single-module `release.json` and mirrors the matching release asset.

## Release safely

- Keep the version in `release.json` aligned with the tag.
- Publish the same tag in the canonical `schwung-mono` repository first.
- Verify the mirrored archive contains `mono-voice/module.json` with the same
  version before publishing it here.
- Do not copy or fork the DSP source into this repository.
