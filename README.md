# WC3 Journal — Android installer

The V10 project starts with **no saved comparisons, Hero Cups, Unit Cups, or Faction Wars**. It retains JSON/older-HTML import and export, private Android app storage, and the Warcraft III icon supplied by the user.

## Build the installable APK

Upload **`WC3_Journal_V10_Android_Source.zip`** to this repository's root (do not extract it). GitHub Actions will automatically launch **Build WC3 Journal APK** after the upload is committed. When it succeeds, open the run and download the **WC3-Journal-V10-Installer** artifact; unzip that artifact and tap `WC3-Journal-V10.apk` on Android. Install with the Android system Package Installer via My Files/Downloads rather than Split APKs Installer (SAI).

The build downloads *exact, verified* classic hero/unit/ability PNG artwork from Warcraft Wiki or Liquipedia Commons, embeds it into the offline HTML, and fails rather than producing an APK with largely missing artwork. It also exports a separate **WC3-Journal-V10-Offline-HTML** artifact containing the artwork.

V10 has a four-emblem faction theme menu, larger distinctive themed navigation icons, no quick-choice buttons or cup merge buttons, and tap-to-study icons. A hero, unit or ability icon opens its associated Liquipedia Warcraft page in the phone's browser. Pages may display balance data from patches newer than WC3 1.26.

Your data resides inside Android private app storage. Export JSON before uninstalling, clearing storage, or installing a version signed with a different debug key. Builds from GitHub's ephemeral debug signing keys may not install as updates over older builds: if Android reports a signature conflict, export first and then uninstall the older app.

This project is a personal, unofficial companion and is not affiliated with Blizzard or Liquipedia.
