# VideoGrab releases

Built binaries for [VideoGrab](https://github.com/TheBiggestPotato/videograb), a native macOS
video downloader. This repository holds **only release artefacts** — the source lives in the
private repository above.

## Install

Download the latest `VideoGrab-<version>.dmg` from [Releases](../../releases), open it, and drag
VideoGrab to Applications. The DMG is signed with a Developer ID certificate and notarized by
Apple, so it opens without any Gatekeeper warning.

Verify the download if you like:

```
shasum -a 256 -c VideoGrab-<version>.dmg.sha256
```

## Updates

Installed copies update themselves through [Sparkle](https://sparkle-project.org), reading
`appcast.xml` from this repository's GitHub Pages site. Every update is checked against both an
EdDSA signature and the Developer ID signature before it is applied.

## Requirements

macOS 14 or later. Apple Silicon and Intel.
