# WC3 Journal — Android installer

This repository builds an installable Android APK from the prepared WC3 Journal source archive.

## Build

Upload `WC3_Journal_AndroidStudio_Source.zip` to the repository root. GitHub Actions will build the Android APK automatically after the ZIP is committed, or you can run **Actions → Build WC3 Journal APK → Run workflow**.

When the workflow finishes, open its run and download the `WC3-Journal-APK` artifact. Unzip that artifact to obtain `WC3-Journal.apk`, then open it on your Android phone and install it.

The source archive has a clean starting database (no previous comparisons, Hero Cups, Unit Cups, or Faction Wars), includes the user-provided icon, and supports import/export of prior Codex backups. The app's data is kept in Android private storage. Keep JSON backups before uninstalling or clearing storage.

This is a debug-signed APK intended for personal sideloading. Do not distribute it as an official Blizzard product.
