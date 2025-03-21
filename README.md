# Bolt's Google Maps Scraper Update System

This repository hosts the update notification system for Bolt's Google Maps Scraper Pro extension.

## How It Works

The `update.json` file contains the latest version information and is accessed by the extension to check for updates.

## Current Version Structure

The update.json file contains:

```json
{
  "version": "2.0.0",
  "downloadUrl": "https://boltscraper.com/downloads/google-maps-scraper-pro-latest.zip",
  "releaseDate": "2023-08-15",
  "releaseNotes": "• Added license deactivation feature\n• Fixed CSS loading delay\n• Enhanced security features\n• Performance improvements",
  "minVersion": "1.0.0"
}
```

## Update Process for Users

1. When the extension starts, it checks this file for version updates
2. If a newer version is available, users are notified with a popup
3. Users can click to download and install the latest version
4. The extension maintains its data across updates

## For Developers

To update the extension:
1. Update the extension code and increase version number in manifest.json
2. Package the new extension
3. Update the update.json file with new version info
4. Commit and push changes to this repository
