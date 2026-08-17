# Homebrew Nodebay

Official Homebrew tap for [Nodebay](https://github.com/Kian-hdr/nodebay), the local-first utility bay in your Mac's notch.

## Install

```bash
brew tap Kian-hdr/nodebay
brew install --cask nodebay
```

Equivalent fully qualified command:

```bash
brew install --cask Kian-hdr/nodebay/nodebay
```

The cask supports Apple Silicon and macOS 15 Sequoia or later. It downloads the signed and notarized archive from the matching [Nodebay GitHub release](https://github.com/Kian-hdr/nodebay/releases) and installs exactly one application: `Nodebay.app`.

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

The public tap will be created only after the exact release and cask receive final approval.
