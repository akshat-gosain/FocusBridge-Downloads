# FocusBridge Downloads

Public installers and release notes only. FocusBridge application source, server credentials,
pairing links, device logs and developer archives do not belong in this repository.

**Release preparation is in progress. No public installer or TestFlight invitation is available yet.**
Do not use historical development-signed disk images as a public release.

## Mac Installation

The release will provide one signed, Apple-notarized package per Mac architecture:

- `macOS-arm64.pkg`: Apple silicon (M-series Macs).
- `macOS-x86_64.pkg`: Intel Macs.

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
