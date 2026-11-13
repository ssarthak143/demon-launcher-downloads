# Demon Launcher downloads

This repository holds **release downloads only**. The Windows and Android development repositories are private. The launchers check the latest published release when they start, and show a prompt only when a newer version is available. Downloads and installation require the player's choice.

The release asset names are:

- `latest.yml` and its matching signed Windows installer (`Demon-Launcher-<version>-x64-Setup.exe`)
- `android.json` and its matching signed Android APK (`demon-launcher-android-<version>.apk`)
- `demon-launcher-android-source-<version>.tar.gz`, including the Android project's LGPL-covered source and build files, alongside the APK
- `SHA256SUMS.txt`

Development builds are not published here. A release is published only after signing and installation checks pass. Android source archives are provided with APKs to preserve recipients' license rights; see the included license and upstream notices.

If this repository has no published release, both launchers remain usable and update checks cannot offer a download yet.
