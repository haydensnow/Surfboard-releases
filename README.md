# Surfboard

An Arc-style sidebar for Safari: tabs, favorites, profiles, link peeks and media controls
in a card beside the page. Surfboard is a menu-bar app for macOS 14 or later.

## Install

```sh
brew install --cask haydensnow/tap/surfboard
```

Or download Surfboard.zip from the [latest release](https://github.com/haydensnow/Surfboard-releases/releases/latest),
unzip it and move Surfboard.app to Applications.

Starting with 0.3, releases contain a universal app for Apple silicon and Intel Macs,
signed with Developer ID and notarized by Apple. Every release includes a SHA-256
checksum file for its ZIP.

Open Surfboard from Applications. Grant Accessibility, Screen Recording, Full Disk
Access and permission to control Safari through Settings > Permissions. The app has no
Dock icon; its menu is in the menu bar.

## Updates

Surfboard checks this repository through Settings > Updates. It verifies the installed
copy's signing requirement before replacing the app. To update through Homebrew:

```sh
brew update
brew upgrade --cask --greedy haydensnow/tap/surfboard
```

If you used a locally signed build from before 0.3, install 0.3 manually or through
Homebrew once and grant the macOS permissions again. Those older copies intentionally
reject the new Developer ID signature. Later releases use the same Developer ID team
and app identifier.

The application source is maintained separately; this public repository hosts releases.
The [Homebrew tap](https://github.com/haydensnow/homebrew-tap) contains the cask only.
