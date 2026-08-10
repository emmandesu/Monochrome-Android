<div align="center">

# Monochrome Android

### A streamlined Android WebView app for Monochrome

Native Android media controls • Foreground/background audio • Downloads • Fullscreen playback

[![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?logo=android&logoColor=white)](#)
[![Distribution](https://img.shields.io/badge/Download-GitHub%20Releases-181717?logo=github)](#downloads)
[![Source](https://img.shields.io/badge/Source-Not%20Published-lightgrey)](#about-this-repository)

</div>

---

## 📱 About

**Monochrome Android** is an Android WebView application designed to provide a more app-like experience for Monochrome on Android.

Instead of being a simple browser wrapper, the app integrates selected Android-native features so media playback, audio controls, downloads, fullscreen content, and background playback behave more naturally on a phone or tablet.

> **This repository is used as the public project and release page for the Android application.**
>
> The application source code is not published in this repository. APK builds are distributed through **GitHub Releases**.

---

## 🌐 Monochrome Web Project

This Android app is built around the Monochrome web experience.

- **Website:** https://monochrome.tf
- **Official Monochrome GitHub repository:** https://github.com/monochrome-music/monochrome

> Monochrome Android is a separate Android WebView application and is not the official Android client of the Monochrome web project unless explicitly stated otherwise.

---

## ✨ Features

<table>
<tr>
<td width="50%" valign="top">

### 🎵 Native Media Controls

Media playback integrates with Android's native media system.

- Play / pause controls
- Previous / next controls when supported
- Media title and playback information
- Lock-screen controls
- Notification media controls
- Bluetooth headset/media-button support
- Android system media panel integration

</td>
<td width="50%" valign="top">

### 🔊 Foreground & Background Audio

Audio can continue playing while the app is no longer in the foreground.

- Android foreground playback service
- Persistent media notification
- Background audio playback
- Screen-off playback
- Playback control without reopening the app
- Better compatibility with Android background restrictions

</td>
</tr>

<tr>
<td width="50%" valign="top">

### ⬇️ Downloads

The app includes Android download handling for supported files and media.

- Download supported content directly from the WebView
- Android download notifications
- File-name and MIME-type handling
- Downloads remain available outside the app
- Uses Android's native download experience where applicable

</td>
<td width="50%" valign="top">

### 🎬 Media & Fullscreen

Designed to make browser-based media feel more native.

- HTML5 audio/video playback
- Fullscreen video support
- Landscape playback support
- Media-session integration
- Playback state synchronization
- Improved handling of media while navigating inside the app

</td>
</tr>

<tr>
<td width="50%" valign="top">

### 🌐 Android WebView

Built around the Android WebView engine for compatibility with modern websites.

- Modern website rendering
- JavaScript support
- Cookies and session support
- In-app navigation
- External-link handling
- File chooser/upload support where supported by the website

</td>
<td width="50%" valign="top">

### 📲 Android Integration

Additional Android behavior provides a more native app experience.

- System back-navigation handling
- Android notifications
- Open supported external applications
- Web-to-Android media integration
- App lifecycle handling
- Android-native permission handling when required

</td>
</tr>
</table>

---

## 📥 Downloads

Official APK builds are published on the repository's **Releases** page.

<div align="center">

### **Download the latest APK from GitHub Releases**

**Repository → Releases → Latest Release → Assets → APK**

</div>

### Installation

1. Open the latest **GitHub Release**.
2. Expand **Assets** if necessary.
3. Download the `.apk` file.
4. Open the APK on your Android device.
5. Allow installation from the browser or file manager if Android asks for permission.
6. Install or update Monochrome.

> When updating, install the new APK over the existing installation.  
> If the signing key/package identity changes between builds, Android may require the previous version to be removed first.

---

## 🎧 Native Media Experience

When compatible media is playing, Monochrome Android can expose playback to Android's Media Session system.

This allows media to appear in places such as:

- Notification shade
- Lock screen
- Quick Settings media player
- Bluetooth headsets
- Android Auto/media-capable devices where supported
- Connected accessories with media buttons

The Android foreground playback service helps keep active audio playback available when the application is minimized or the screen is turned off.

---

## ⬇️ Download Support

Downloads initiated from supported pages can be handed over to Android's download system.

Depending on the source website and file type, Android may display a download notification and save the file to the device's normal download location.

> Download availability ultimately depends on whether the website exposes a downloadable resource. DRM-protected, streamed, blob-based, encrypted, or otherwise restricted media may not be directly downloadable.

---

## 🔐 Permissions

Depending on the Android version and enabled features, the application may request or use permissions related to:

| Permission / Capability | Purpose |
|---|---|
| Internet access | Load Monochrome and online content |
| Notifications | Media playback and download notifications |
| Foreground service | Keep active media playback running |
| Media playback service | Support foreground/background audio |
| Storage / media access | Used only where required for supported file operations |
| File chooser | Allow websites to request a file from the device |

Android permission behavior may vary depending on the OS version.

---

## 📋 Requirements

- Android device with a compatible **Android System WebView**
- Internet connection
- Notification permission for full media-control functionality on Android versions that require it
- Permission to install APK files when installing outside the Google Play Store

Keeping **Android System WebView** up to date is recommended.

---

## 🚀 Releases

Releases are used to publish:

- New APK versions
- Bug fixes
- Media playback improvements
- Android compatibility updates
- WebView improvements
- Download handling changes
- Release notes and known issues

Each release may include its own changelog and installation notes.

---

## 🐛 Issues & Feedback

If you encounter a problem, open an issue in the repository and include as much useful information as possible.

Recommended information:

- App version
- Android version
- Device model
- Android System WebView version
- Steps to reproduce the problem
- Screenshot or screen recording, if relevant
- Crash log / Logcat output for crashes

### Good issue examples

- Media notification controls do not respond
- Audio stops after locking the screen
- Fullscreen video cannot exit correctly
- Download does not start
- File chooser does not open
- A page fails to load in Android WebView

Please avoid posting account passwords, authentication tokens, cookies, or other private information in issue reports.

---

## ❓ Frequently Asked Questions

<details>
<summary><b>Where can I download the app?</b></summary>

APK files are published in **GitHub Releases**. This repository does not provide APK files through the source-code download buttons.

</details>

<details>
<summary><b>Is the source code available?</b></summary>

No. This repository currently serves as the public information, issue-tracking, and APK release page for Monochrome Android.

</details>

<details>
<summary><b>Why does Android show a persistent notification while audio is playing?</b></summary>

Android requires applications performing ongoing foreground media playback to display a foreground-service notification. This also provides access to native playback controls.

</details>

<details>
<summary><b>Can audio continue when the screen is off?</b></summary>

Yes, foreground/background audio support is designed to allow compatible media to continue playing while the app is minimized or the display is off.

</details>

<details>
<summary><b>Why can't some media be downloaded?</b></summary>

The website must expose a resource that Android can download. Some streams use DRM, encrypted manifests, temporary URLs, JavaScript blobs, or other delivery methods that cannot be handled as a normal file download.

</details>

<details>
<summary><b>Does the app replace Android System WebView?</b></summary>

No. Monochrome Android uses the WebView implementation available on the device.

</details>

---

## 🧩 About This Repository

This repository intentionally contains **no application source code**.

It is maintained for:

- 📦 APK releases
- 📝 Release notes
- 🐛 Issue reports
- 📢 Announcements
- 📚 User documentation

The downloadable application package can be found under **Releases**.

---

## ⚠️ Disclaimer

Monochrome Android is a WebView-based Android client. Website availability, hosted content, external services, and individual media sources are outside the control of the Android application.

Users are responsible for complying with applicable laws, website terms, content licenses, and service policies when using or downloading content.

---

<div align="center">

### Monochrome Android

**Android WebView • Native Media Controls • Background Audio • Downloads**

Check **Releases** for the latest APK.

</div>
