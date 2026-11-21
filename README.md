# FocusBridge Downloads

Public installers and release notes only. FocusBridge application source, server credentials,
pairing links, device logs and developer archives do not belong in this repository.

**Signed Mac installers are available. [Join FocusBridge on TestFlight](https://testflight.apple.com/join/JNZdkMqz).**
Apple's external review is pending, so this public link cannot accept installs yet.
Do not use historical development-signed disk images as a public release.

The App Store listing is **FocusBridge: Earn Your Time**. The first release is free,
with no purchase, subscription or account-access beta cutoff. Each TestFlight build
still has Apple's build expiry. No invitation link will be posted before it exists.

See the [setup/support guide](SUPPORT.md) and [privacy notice](PRIVACY.md).
Support/privacy contact: [akshat.gosain1990@gmail.com](mailto:akshat.gosain1990@gmail.com).

## Mac Installation

Download the signed, Apple-notarized package from the [Mac companion release](https://github.com/akshat-gosain/FocusBridge-Downloads/releases/tag/v0.3.0-beta):

- `macOS-arm64.pkg`: Apple silicon (M-series Macs).
- `macOS-x86_64.pkg`: Intel Macs.

Install the iPhone app from TestFlight once Apple approves the build, then choose
**Continue with Apple**. Follow **Connect your Mac** in the iPhone setup to install
the companion and connect both devices to that account. Mac installation alone
does not create an account. App Store review and release are separate.

Open the package and complete the standard macOS installer. It installs FocusBridge and the
official ActivityWatch collector into Applications. No Terminal commands or Xcode are needed.
Open FocusBridge, then use Connect your Mac on the iPhone to send its private one-use link.
Confirm the connection on the Mac. Grant ActivityWatch Accessibility permission when requested,
choose productive apps, and optionally enable launch at login. Permissions remain your choice.

macOS 14 or later is required. The iPhone app requires iOS 17.4 or later.
Windows is not supported in this release.

## Third-Party Software

ActivityWatch is an independently developed, open-source application, not a hidden service.
Its original signature is preserved. See THIRD_PARTY_NOTICES.txt for upstream source and licensing.
