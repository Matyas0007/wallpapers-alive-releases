# Wallpapers Alive

Your own videos as the macOS desktop wallpaper, and optionally on the Lock Screen.

Wallpapers Alive is a tiny menu-bar app that plays videos you choose as a live wallpaper on every display. Import a
clip once and it is optimized for cheap, hardware-decoded looping; playback pauses whenever nobody can see it. It is
native, has no third-party dependencies and no Dock icon.

**[Download the latest release](https://github.com/Matyas0007/wallpapers-alive-releases/releases/latest)**

## Download

| File | System | What it is |
| --- | --- | --- |
| `Wallpapers-Alive-X.Y.Z.dmg` | macOS 26 or later, Apple silicon | The installer. **Download this.** |
| `latest-mac.json`, `Wallpapers-Alive-X.Y.Z.zip` | macOS | Update files that installed copies read |

You never need to download the update files yourself.

## Requirements

- macOS 26 or later on an Apple silicon Mac.

## Install

Open the `.dmg`, drag **Wallpapers Alive** onto **Applications**, and start it from Applications. The icon appears in
the menu bar; choose **Add Videos…** to start. The app is signed with a Developer ID and notarized by Apple, so it
opens without a warning. Keep it in Applications so it can update itself.

## Updates

Wallpapers Alive (1.3.0 and later) updates itself from this page. The menu bar has **Check for Updates…** and
**Check Automatically** (on by default): a few seconds after launch and then every 4 hours, it reads
`latest-mac.json` from the newest release. It only looks; when there is a newer version, nothing downloads until you
click **Download**, and then **Restart to Update** installs it.

- The download is checked against the SHA-512 in `latest-mac.json`.
- The update is installed only if it is signed with the same Developer ID as the app you are running.

Versions before 1.3.0 don't check for updates: install 1.3.0 or later once from the `.dmg`. Updates replace only the
app: your library and settings stay as they are.

## Uninstall

Quit Wallpapers Alive and drag it from Applications to the Trash.

What stays: its own data in `~/Library/Application Support/Wallpapers Alive` (your library and the backup of your
macOS wallpaper settings), which you can delete yourself.

Before you uninstall, choose **Restore macOS Wallpaper…** in the menu if you used the Lock Screen option or
**Match Menu Bar to Video**: they work through macOS's own wallpaper settings, and this puts yours back. On macOS 27.2
the Lock Screen option is unavailable, because macOS no longer loads custom Lock Screen videos.

## Privacy

- No analytics, no telemetry, no crash reporter, no account.
- The only network request is the update check: it reads `latest-mac.json` from this repository's releases, and
  downloads an update only when you click Download.
- Your videos never leave your Mac.

## About this page

This repository holds only Wallpapers Alive's installers and update files. The source code is private.

## License

Wallpapers Alive is © 2026 Matyas Kucera. **All rights reserved.** It is not open source.
