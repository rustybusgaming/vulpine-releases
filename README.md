# Vulpine

A privacy browser built on Chromium. It blocks ads, trackers and fingerprinting
before a request leaves your machine, and lists exactly what it stopped.

**Website and documentation: https://vulpine.lol**

## Download

The installers are on the [Releases](../../releases) page, for Windows, macOS
(one app for Apple silicon and Intel) and Linux (AppImage, or a .deb for Debian
and Ubuntu). Each release lists every file with its size and SHA-256 checksum.

Vulpine updates itself from these releases on Windows and from the AppImage. On
a Mac, and from the .deb, it tells you when a new version is out.

## What this repository is

Releases only. The source code is not published here: this repository exists so
that anyone can download Vulpine, check a file against its published checksum,
and see every version that has been released. Installed copies of Vulpine read
the same releases to find updates.

## Opening it the first time

Neither the Windows installer nor the Mac app is code-signed yet.

- **Windows**: SmartScreen says it protected your PC. Choose **More info**, then
  **Run anyway**.
- **macOS**: open **System Settings**, **Privacy & Security**, and choose
  **Open Anyway**.

## Checking a download

```
Get-FileHash .\<file> -Algorithm SHA256     # Windows, in PowerShell
shasum -a 256 <file>                          # macOS
sha256sum <file>                              # Linux
```

The result should match the checksum listed with the release.

## Privacy

Vulpine sends no analytics, telemetry or crash reports. The privacy policy lists
every request the browser makes: https://vulpine.lol/privacy.html

---

This README is kept up to date by the release process; changes made here
directly are replaced on the next release.
