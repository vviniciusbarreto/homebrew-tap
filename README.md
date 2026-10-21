# Vinicius Barreto Homebrew Tap

This directory contains the source for the public `vviniciusbarreto/homebrew-tap` repository.

## WhatsClean

### WhatsClean 1.1.3 — clearer confirmation and localization

- Moving selected files to the Trash now shows the number of files and the space you will recover before you confirm.
- The WhatsApp folder access window and its alerts follow your macOS language, including Brazilian Portuguese.
- Regression tests use only synthetic files and can no longer reach a real WhatsApp folder authorization; automated macOS checks run on every change.

Automatic cleanup, scheduling, and Trash behavior are unchanged. [Full release notes](https://github.com/vviniciusbarreto/WhatsClean/releases/tag/v1.1.3).

To receive the update notice and release notes, open WhatsClean with automatic update checks enabled, or use **Check for Updates**. A fully quit app runs only its scheduled cleanup; it does not check for updates.

Install:

```bash
brew install --cask vviniciusbarreto/tap/whatsclean
```

Upgrade:

```bash
brew update
brew upgrade --cask whatsclean
```

Update `version` and `sha256` in `Casks/whatsclean.rb` for every release.

## UniDownloader

A private native macOS interface for yt-dlp for Apple Silicon, with menu bar URL drops, bundled FFmpeg/FFprobe, and signed automatic updates. Requires macOS Sequoia or later; the cask installs Deno for YouTube JavaScript challenge support. UniDownloader replaces YTDLP Glass and keeps its bundle identifier, so YTDLP Glass 1.0.0 installs update in place through Sparkle.

Install:

```bash
brew install --cask vviniciusbarreto/tap/uni-downloader
```

Upgrade:

```bash
brew update
brew upgrade --cask uni-downloader
```

Update `version` and `sha256` in `Casks/uni-downloader.rb` for every release.

UniDownloader and WhatsClean have separate repositories, releases, casks, and descriptions.
