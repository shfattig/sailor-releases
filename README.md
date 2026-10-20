# Sailor releases

Download Sailor for Android from this repository's Releases page, or let
[Obtainium](https://github.com/ImranR98/Obtainium) install and update it for
you. This repository hosts release binaries and documentation. Sailor's
application source is maintained privately.

## Install and update with Obtainium (recommended)

1. Install Obtainium, then add Sailor with this link from your phone:
   [obtainium://add/https://github.com/shfattig/sailor-releases](obtainium://add/https://github.com/shfattig/sailor-releases)
   (or in Obtainium: Add App → `https://github.com/shfattig/sailor-releases`).
2. Set **Filter APKs by regular expression** to `sailor-stable-.*-arm64\.apk`.
   Releases also carry Linux desktop files; this picks the Android app.
3. Beta testers: turn on **Include prereleases**. Betas are published as GitHub
   pre-releases as soon as they're built; with the option off you get stable
   releases only.

Obtainium then checks for new releases and updates Sailor in place. Betas and
stable releases are the same app, signed with the same key, so you can switch
between channels without reinstalling or losing data.

## Manual installation

Download the `sailor-stable-…-arm64.apk` asset to an ARM64 Android device running
Android 7.0 or newer. Allow installation from your browser or file manager when
Android asks. Later APKs update the same app without uninstalling it.

Stable Sailor uses the Android application ID `io.sailor`. Sailor Dev is a
separate local deployment using `io.sailor.dev`.

Each release includes a SHA-256 checksum and metadata with the package ID,
version code, and signing certificate fingerprint. Download the APK and its
`.sha256` file into the same directory, then verify with `sha256sum -c FILE.sha256`.

## Keep your devices on the same version

Sailor syncs peer to peer. Occasionally a release changes how devices sync, and
its release notes say so; update every device you sync with to that release.
Obtainium makes this quick.

Before replacing an older Flutter installation, back up your data and follow
the migration instructions in the release notes. The new app reuses an existing
Flutter sailor-core store; Flutter-only settings may need to be configured again.
