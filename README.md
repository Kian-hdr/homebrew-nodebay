# Homebrew Nodebay

Official Homebrew tap for [Nodebay](https://github.com/Kian-hdr/nodebay), the local-first utility bay in your Mac's notch.

## Install

```bash
brew tap Kian-hdr/nodebay
brew trust --cask Kian-hdr/nodebay/nodebay
brew install --cask nodebay
```

Homebrew 6 requires the one-time trust command for casks from third-party taps. This trusts only the Nodebay cask. After that, the equivalent fully qualified command is:

```bash
brew install --cask Kian-hdr/nodebay/nodebay
```

The cask supports Apple Silicon and macOS 15 Sequoia or later. Once the first release is published, it will download the signed and notarized archive from the matching [Nodebay GitHub release](https://github.com/Kian-hdr/nodebay/releases) and install exactly one application: `Nodebay.app`.

## Upgrade

```bash
brew update
brew upgrade --cask nodebay
```

## Uninstall

```bash
brew uninstall --cask nodebay
```

To also remove Nodebay preferences and caches:

```bash
brew uninstall --cask --zap nodebay
```

Zap does not delete original shelf files, downloads, generated Markdown, or compressed image outputs.

## Project links

- [Source](https://github.com/Kian-hdr/nodebay)
- [GPL-3.0 license](https://github.com/Kian-hdr/nodebay/blob/main/LICENSE)
- [Privacy](https://github.com/Kian-hdr/nodebay/blob/main/PRIVACY.md)
- [Security](https://github.com/Kian-hdr/nodebay/blob/main/SECURITY.md)
- [Issues](https://github.com/Kian-hdr/nodebay/issues)

Nodebay is based on [Boring Notch](https://github.com/TheBoredTeam/boring.notch) commit `44dd999f70493da48209c99e9f873c47f2e55c83`. This tap is not affiliated with or endorsed by Apple, Microsoft, Spotify, YouTube, ImageOptim, or other integrated providers.

Release artifacts and cask checksums are published together only after Developer ID signing, Apple notarization, stapling, and installation verification.
