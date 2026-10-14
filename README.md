# Sailor releases

Download the latest stable Sailor Android APK from this repository's Releases
page. This repository hosts release binaries and documentation. Sailor's
application source is maintained privately.

## Android installation

Download the `sailor-stable-…-arm64.apk` asset to an ARM64 Android device running
Android 7.0 or newer. Allow installation from your browser or file manager when
Android asks. Later stable APKs update the same app without uninstalling it.

Stable Sailor uses the Android application ID `io.sailor`. Sailor Dev is a
separate local deployment using `io.sailor.dev`.

Each release includes a SHA-256 checksum and metadata with the package ID,
version code, and signing certificate fingerprint. Download the APK and its
`.sha256` file into the same directory, then verify with `sha256sum -c FILE.sha256`.

Before replacing an older Flutter installation, back up your data and follow
the migration instructions in the release notes. The new app reuses an existing
Flutter sailor-core store; Flutter-only settings may need to be configured again.
