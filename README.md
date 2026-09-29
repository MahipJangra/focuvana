# Focuvana

A simple Android focus timer with optional app blocking, custom durations, and session history.

## Download and install

1. Open the **Releases** section of this GitHub repository.
2. Open the latest release and expand **Assets**.
3. Download the file ending in **.apk**, such as `Focuvana-v0.1.0.apk`.
4. Open the downloaded APK on your Android phone.
5. If Android asks, allow **Install unknown apps** for the browser or file manager you used. The wording varies by phone.
6. Tap **Install**, then open **Focuvana**.

Requires **Android 8.0 or newer**. You do not need Android Studio or a computer to install the APK. Download the APK asset, not GitHub's automatically generated source-code ZIP.

## Use the timer

- Choose **25**, **45**, or **60 minutes**, or tap **Custom duration** to enter 1–720 minutes.
- Turn **Focus mode OFF** to use the timer without blocking apps.
- Tap **Start timer** or **Start focusing** to begin.
- Tap **End session** to stop early.
- Open **Progress** to view saved sessions.

## Set up app blocking

1. Open the **Apps** tab and select the apps you want to block.
2. On the **Focus** tab, tap **Set up blocking permission**.
3. Read the permission explanation, then open Android Settings.
4. Find **Focuvana focus protection** under Accessibility / Installed apps (the service may still be labelled **Reclaim focus protection** in older builds).
5. Enable the service and return to Focuvana.
6. Turn **Focus mode ON** and start a timer.

During an active session, opening a selected app returns you to your home screen. Turn **Focus mode OFF** at any time to stop blocking without stopping the timer. Your accessibility permission stays enabled, so you do not need to grant it again for every session.

The service checks which app opens to provide blocking. It does not request access to read screen content. App selections and session history are stored locally; this version has no account or network permission.

## If Android blocks the accessibility setting

Some Android phones restrict accessibility access for apps installed from downloaded APKs. If you see **Restricted setting**, open **Settings → Apps → Focuvana**, then check the three-dot menu for **Allow restricted settings**. Only enable this if you trust the APK and its source. Return to Accessibility settings afterward. Menu names and availability vary by device.

## Updating

Download the newer APK from Releases and install it over the existing app. Updates must use the same app ID and signing key to preserve an existing installation.

If you previously installed a development/debug build from Android Studio, the release APK may use a different signing key. Android may require you to uninstall that earlier build first. **Uninstalling deletes its saved app data and history.**

## Troubleshooting

- **Apps are not blocked:** Check that Focus mode is ON, a timer is running, at least one app is selected, and the accessibility service is enabled.
- **Timer only:** Switch Focus mode OFF. You do not need to disable accessibility permission.
- **App not installed:** Check that your device runs Android 8.0 or newer, that the download completed, and that there is no conflicting installation signed with another key.

## Early release

Focuvana is an early version. App blocking is a return-to-home action, not an unbreakable device lock. Behaviour may vary by phone. Daily screen-time limits, scheduled sessions, and completion notifications are not included yet.

This repository provides the Focuvana Android APK for download. The source code is not publicly included. To request access, contact **mahipjangra8@gmail.com**.
