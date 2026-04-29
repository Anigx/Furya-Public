# Privacy Policy

## Overview

Furya is a closed-source Android application. It does not operate its own servers. All data is stored locally on your device or sent directly to the content sources you choose (e621 or e6ai).

## Data Stored Locally

Furya stores the following data locally on your device:

- **API keys** – used to authenticate your account with e621 or e6ai
- **Account preferences** – source selection, display settings, filters
- **Local favorites** – when not connected to an account
- **Collections** – posts you have saved to collections
- **Blacklist entries** – tags and rating filters you have configured
- **Offline cache** – cached posts and tag data for offline use
- **Downloaded media** – files you have downloaded to device storage
- **Search history** – recent searches for convenience
- **Usage statistics** – if you have enabled optional anonymous telemetry

## API Keys and Account Data

API keys are stored locally on your device. They are used only to authenticate requests to the selected content source (e621 or e6ai). Furya does not send your API key to the developer.

We recommend protecting your device with a lock screen (PIN, password, or biometric) and removing your account from Furya before selling or giving away your device.

## Data Sent to e621/e6ai

When you use Furya, it sends requests directly to e621.net or e6ai.net APIs. This includes:

- Search queries and tag searches
- Favorite and pool operations
- Post downloads
- Account authentication

This communication is between you and the content source directly.

## Data Sent to GitHub for Update Checks

Furya checks GitHub Releases for available updates. This check only sends your current app version number to GitHub. No personal data or account information is transmitted.

## Data Sent to the Developer

**Furya does not send usernames, API keys, search queries, favorites, viewed posts, downloaded files, collections, or blacklist entries to the developer.**

## Anonymous Usage Statistics

Anonymous usage statistics are optional and disabled by default. If enabled, they collect only anonymous, non-personal information such as:

- App feature usage (e.g., which screens are opened)
- General app performance metrics
- Crash reports (without personal data)

**Anonymous statistics do NOT include:**

- Usernames or API keys
- Search queries or tags
- Favorites or blacklist entries
- Downloaded files or post IDs
- Collection contents

You can enable or disable usage statistics at any time in Settings.

## Local Cache and Downloads

Media files you download and cached data are stored in your device's app storage. These files remain on your device until you manually delete them or uninstall Furya.

## Data Deletion

To delete your local data:

1. **Remove your account** – Go to Settings > Accounts and remove your e621/e6ai account
2. **Clear the cache** – Go to Settings > Storage and clear the app cache
3. **Delete downloaded files** – Use a file manager to navigate to Android/data/com.furya.app/ and delete the files folder
4. **Uninstall the app** – This removes all data stored by Furya

## Security

- API keys are stored only on your device
- Use a device lock screen (PIN, password, biometric) for additional protection
- Never share your API key with anyone
- Do not post your API key in public issues or support requests

## Third-Party Services

Furya communicates directly with:

- **e621.net** – for e621 API access
- **e6ai.net** – for e6ai API access
- **GitHub** – for release updates only

No data is sent to any other third-party services.

## Contact

For privacy-related questions, please [open an issue](https://github.com/Anigx/Furya-Public/issues) on GitHub.