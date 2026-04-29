<div align="center">
  <img src="assets/furya_logo.png" alt="Furya Logo" width="180" height="180">
</div>

# Furya

Fast, native Android client for e621 and e6ai.

**Furya is currently distributed as a closed-source Android app.**

This public repository provides release downloads, update information, documentation, and a place to report bugs or request features. The app source code is not published here.

[![Latest Release](https://img.shields.io/github/v/release/Anigx/Furya-Public?style=for-the-badge&color=00796b&label=Download%20APK)](https://github.com/Anigx/Furya-Public/releases/latest)

[![Built with Flutter](https://img.shields.io/badge/Built%20with-Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)](https://flutter.dev)
![Platform Android](https://img.shields.io/badge/Platform-Android-3DDC84?style=flat-square&logo=android&logoColor=white)

## Overview

Furya is a native Android app focused on fast browsing, smooth media playback, and reliable account sync for large collections.

It is built as an app-first experience, not a web wrapper.

## Current Feature Set

### Feed and Navigation

- Infinite masonry feed with prefetching and pagination.
- Pull to refresh and automatic load more.
- Scroll position memory per query and feed context.
- Quick scroll-to-top button for long sessions.
- Configurable grid columns (1, 2, or 3).

### Search, Filters, and Discovery

- Tag search with chip-based query building.
- Local tag cache plus API fallback for autocomplete.
- Favorite tags picker and favorite tag management.
- Tag groups for organizing favorite tags.
- Filter sheet with sort modes and rating filters.
- Popular mode with day, week, and month ranges.
- Search history support.

### Content Sources and Accounts

- Source switch: e621, e6ai, or mixed mode.
- Separate account handling for e621 and e6ai.
- Guest mode support for e621.
- API key based login flow with in-app help.

### Media Viewer

- Fullscreen post viewer with swipe navigation.
- Deep zoom for images via interactive viewer.
- HD viewer mode and progressive high-resolution upgrade.
- Native WebM and MP4 playback.
- GIF playback support.
- Slideshow mode with adjustable speed.
- Shuffle mode inside the viewer.
- Fullscreen immersive mode toggle.
- Download media directly to device storage.
- SWF fallback with external browser opening.
- Landscape option to hide info overlays.

### Favorites and Sync

- Source-aware favorites for e621 and e6ai.
- Automatic account sync when a source account is connected.
- Local fallback favorites when no account is connected.
- Mixed mode favorites tabs (e621 and e6ai split).
- Local favorites search, sort, and rating filters.
- Pool-aware favorite flow that can also save full comic pools.

### Pools

- Browse pools with search, sort, and category filters.
- Toggle between list and grid pool views.
- Open pool detail pages with ordered posts.
- Favorite and unfavorite pools from list and detail views.

### Collections

- Create, rename, delete, and reorder collections.
- Save posts to collections from the post viewer.
- Multi-select collection management.
- Export collections as JSON.
- Import collections from JSON.

### Favorite Artists

- Dedicated favorite artists tab.
- Search within favorite artists.
- Open an artist directly as a filtered feed.

### Blacklist and Safety

- Local blacklist management UI.
- Source-specific blacklist handling (e621, e6ai, both).
- Sync blacklist tags from remote APIs.
- Import and export blacklist data.
- Remove entries individually or clear by source.
- Safe mode rating filters.

### Offline, Cache, and Data

- Offline tag rules for background caching.
- Manual offline sync trigger.
- Storage limit configuration for offline cache.
- Tag database update screen with progress and ETA.
- Connectivity status indicator and offline awareness.

### App Maintenance

- In-app update check against GitHub releases.
- In-app APK download flow for updates.
- App version/build info in settings.
- Optional anonymous usage statistics toggle.

## Installation

1. Open the [latest release page](https://github.com/Anigx/Furya-Public/releases/latest).
2. Download the attached APK file (`Furya-vX.X.X-bNN.apk`).
3. Install the APK on Android. This is a universal build and works on all supported devices.

**Only download Furya from the official GitHub Releases page or through the in-app updater.**

## Content Warning

Furya can display content from e621 and e6ai, including mature or explicit material depending on user settings and source content. Users are responsible for configuring filters, blacklists, and safe mode according to their preferences and local laws.

## Disclaimer

Furya is a third-party client for public APIs provided by e621.net and e6ai.net.



## Star History

[![Star History Chart](https://api.star-history.com/chart?repos=Anigx/Furya-Public&type=timeline&logscale&legend=top-left)](https://www.star-history.com/?repos=Anigx%2FFurya-Public&type=timeline&legend=top-left)

## Disclaimer

Furya is not affiliated with, endorsed by, or sponsored by e621 or e6ai.
