# Homebrew Nodebay

Official Homebrew tap for [Nodebay](https://github.com/Kian-hdr/nodebay), the local-first utility bay in your Mac's notch.

## Set up with your AI agent

**[Copy the setup prompt into your agent's chat](SETUP-PROMPT.md).** No placeholders
need editing. Use an agent with access to your Mac; it will check compatibility,
download and verify the installer, preserve existing settings, and guide any
permissions or configuration you need to complete yourself.

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

The cask supports Apple Silicon and macOS 15 Sequoia or later. It downloads the signed, notarized, and stapled DMG from the matching [Nodebay GitHub release](https://github.com/Kian-hdr/nodebay/releases) and installs exactly one application: `Nodebay.app`. The unmodified yt-dlp and FFmpeg Homebrew formulas are installed as separate companion dependencies for local media downloads and processing.

Nodebay 1.2.0 adds optional Quick Chat with clear API-key setup and text-fitting message bubbles, available media-source tabs, and file-drawer fixes. Quick Chat defaults to Off. OpenAI API billing is separate from a ChatGPT subscription; API keys are stored in macOS Keychain. Codex CLI and Longhaul are optional separate integrations and are not installed by this cask. ImageOptim and Blender 5.0.1 are optional, separately installed apps, not cask dependencies. See the application's [feature documentation and limitations](https://github.com/Kian-hdr/nodebay#features) and [release verification](https://github.com/Kian-hdr/nodebay/blob/main/docs/release-verification-matrix.md); installation does not establish physical-display or per-site downloader compatibility.

For guided, data-preserving installation and optional AI setup, use the
[setup prompt](https://github.com/Kian-hdr/nodebay/blob/main/SETUP-PROMPT.md).

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

Zap does not delete original shelf files, downloads, Quick Notes, generated Markdown, repaired STL files, or compressed outputs. It intentionally preserves Nodebay's Application Support storage and backups.

## Project links

- [Source](https://github.com/Kian-hdr/nodebay)
- [GPL-3.0 license](https://github.com/Kian-hdr/nodebay/blob/main/LICENSE)
- [Privacy](https://github.com/Kian-hdr/nodebay/blob/main/PRIVACY.md)
- [Security](https://github.com/Kian-hdr/nodebay/blob/main/SECURITY.md)
- [Issues](https://github.com/Kian-hdr/nodebay/issues)

Nodebay is based on [Boring Notch](https://github.com/TheBoredTeam/boring.notch) commit `44dd999f70493da48209c99e9f873c47f2e55c83`. This tap is not affiliated with or endorsed by Apple, Microsoft, Spotify, YouTube, ImageOptim, or other integrated providers.

Release artifacts and cask checksums are published together only after Developer ID signing, Apple notarization, stapling, and installation verification.
