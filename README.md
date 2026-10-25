# HEAV3NS-CODE native macOS releases

Official binary distribution channel for the native HEAV3NS-CODE workspace for LUMI.
The [application source](https://github.com/CardSorting/HEAV3NS-CODE) is maintained separately.

## Install

Download the matching Apple Silicon or Intel DMG from [Releases](https://github.com/CardSorting/HEAV3NS-CODE-Releases/releases).
Requires macOS 14 or later. Open the DMG, drag HEAV3NS-CODE to Applications, and
launch normally. Public app and DMG packages are Developer ID signed, notarized,
and stapled. No quarantine removal or Gatekeeper bypass is required.

Each release includes both architecture DMGs and ZIPs, `SHA256SUMS.txt`, and a
verified `install.sh`. Compare downloads with the checksum manifest.

For native 15.0.2, download and review the installer before running:

```sh
curl --proto '=https' --proto-redir '=https' -fsSL https://github.com/CardSorting/HEAV3NS-CODE-Releases/releases/download/v15.0.2/install.sh -o heav3ns-install.sh
bash heav3ns-install.sh v15.0.2
```

`bash heav3ns-install.sh --check` checks for updates without replacing your app.
The installer verifies the archive, Apple signing identity, version, architecture,
and Gatekeeper acceptance. It never stops an active app or downgrades it, and
keeps a prior installation for rollback.

## Native updates

Choose HEAV3NS-CODE → Check for Updates…, or enable automatic checks and optional
downloads in the app menu. Updates wait for active workspace work and unsaved edits.
The app, Node runtime and engine update together as a signed bundle. Existing
Apple Silicon installations keep a migration path through their original feed;
the update-signing key is preserved.

See [UPDATES.md](UPDATES.md) for the release pipeline, signed-feed policy, and recovery.
Website: [heav3ns.com/code](https://heav3ns.com/code).

License and third-party notices are included here and in every app bundle.
