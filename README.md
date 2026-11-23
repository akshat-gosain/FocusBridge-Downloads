# FocusBridge Downloads

Public installers and release notes only. FocusBridge application source, server credentials,
pairing links, device logs and developer archives do not belong in this repository.

**Mac, Windows and Android downloads are available. [Join FocusBridge on TestFlight](https://testflight.apple.com/join/JNZdkMqz).**
The public TestFlight link is open. App Store review and public App Store release
are separate; a TestFlight invitation is not an App Store listing.
Update to **0.3.0 (32)** for guided Mac/Windows downloads and pairing. The earlier
app-selection setup fix is included: choose your apps/categories/websites and tap
**Done** to save.
Do not use historical development-signed disk images as a public release.

The App Store listing is **FocusBridge: Earn Your Time**. The first release is free,
with no purchase, subscription or account-access expiry. Each TestFlight build
still has Apple's build expiry.

See the [setup/support guide](SUPPORT.md) and [privacy notice](PRIVACY.md).
Support/privacy contact: [akshat.gosain1990@gmail.com](mailto:akshat.gosain1990@gmail.com).

## Mac Installation

Download the signed, Apple-notarized package from the [Mac companion release](https://github.com/akshat-gosain/FocusBridge-Downloads/releases/tag/v0.3.0-beta):

- `macOS-arm64.pkg`: Apple silicon (M-series Macs).
- `macOS-x86_64.pkg`: Intel Macs.

Install the iPhone app from TestFlight, then choose
**Continue with Apple**. Follow **Connect your computer → Mac** in the iPhone setup to install
the companion and connect both devices to that account. Mac installation alone
does not create an account. App Store review and release are separate.

Open the package and complete the standard macOS installer. It installs FocusBridge and the
official ActivityWatch collector into Applications. No Terminal commands or Xcode are needed.
Open FocusBridge, then use Connect your computer → Mac on the iPhone to send its private one-use link.
Confirm the connection on the Mac. Grant ActivityWatch Accessibility permission when requested,
choose productive apps, and optionally enable launch at login. Permissions remain your choice.

macOS 14 or later is required. The iPhone app requires iOS 17.4 or later.

## Windows Installation

Download [FocusBridge for Windows x64](https://github.com/akshat-gosain/FocusBridge-Downloads/releases/tag/windows-v0.3.0).
The setup EXE includes the .NET runtime and official ActivityWatch collector; no
SDK, Terminal commands or separate collector installation is needed. Windows 10
version 2004 or later, or Windows 11, is required.

The Windows installer is currently **unsigned**. Windows may warn about or block
it. Its release page includes the signing status, SHA-256 and native check results.
Do not disable Windows security protections. A real-PC foreground/idle/browser
acceptance check is still outstanding.

iPhone build **32** is available through the public TestFlight link and adds
installer links and Windows pairing. Historical build 30 supports Mac setup only.
In the updated iPhone app choose **Settings →
Connect your computer → Windows**, send the installer link to your PC, then create
a private connection link/code. Open FocusBridge on Windows and confirm Connect.

A Mac and a Windows PC can both contribute to one account. Productive seconds from
different computers are combined, with simultaneous intervals counted once, not
twice. Each computer needs its own one-use connection link. Adding Windows does
not disconnect a Mac or reset the phone balance. See [Windows setup](WINDOWS_SETUP.md).

## Android Installation

[Download FocusBridge for Android](https://github.com/akshat-gosain/FocusBridge-Downloads/releases/tag/android-v0.3.0)
and follow the [Android setup guide](ANDROID_SETUP.md). The release-signed APK
requires Android 10 or later and includes guided account creation, permissions,
app selection and Mac/Windows pairing. One Android or iPhone spends an account's
balance; Mac and Windows can both contribute. No Android hardware was available
for physical acceptance; the release records that limit rather than claiming it
was tested on a phone. This APK is not a Google Play release.

## Third-Party Software

ActivityWatch is an independently developed, open-source application, not a hidden service.
Its original signature is preserved. See THIRD_PARTY_NOTICES.txt for upstream source and licensing.
