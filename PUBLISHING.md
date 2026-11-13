# Publishing a verified update

The launchers check this repository's public `updates` release on startup. Keep the Windows and Android source repositories private. Only upload builds that have passed signing and device checks.

## Windows

Prepare a signed draft with the private Windows repository's **Prepare signed Windows release** workflow. Confirm the installer has a valid Authenticode signature from the expected publisher and that its version is newer than the last published installer. Upload the installer first, then its matching `latest.yml` last. The launcher checks the metadata, verifies the download hash and the expected publisher, and asks the player before downloading or installing.

## Android

Prepare a private draft with the Android repository's **Prepare signed Android release** workflow. Test a clean install, a same-key upgrade, a real game launch, touch joystick, mouse/keyboard, and the x86_64 emulator. Upload the signed APK and matching LGPL source archive together. Upload `android.json` last so no player sees metadata for an APK that is not present yet. Keep the matching `SHA256SUMS.txt` available.

This release is intentionally empty until the first signed, verified build is ready. A source-code archive accompanies every Android APK even though the development repository remains private.
