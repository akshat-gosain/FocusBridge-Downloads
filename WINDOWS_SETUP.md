# FocusBridge for Windows

This x64 package includes FocusBridge, its .NET runtime, and the unmodified official
ActivityWatch 0.14.3 collector. No SDK or separate ActivityWatch installation is needed.
Use Windows 10 version 2004 or later, or Windows 11. Native ARM64 is not claimed.

**Signing status:** This publicly downloadable installer is currently unsigned.
Windows may warn about or block it. See `verification.json` for its signing status
and SHA-256. Do not disable Windows security protections to install it. Native
installation checks passed; physical foreground/idle/browser acceptance on a user's
Windows PC is still outstanding.

## Connect

1. Run `FocusBridge-Windows-x64-Setup.exe`, then open FocusBridge.
2. In iPhone build 32 or later, choose Settings → Connect your computer → Windows.
   Create a connection link and send it privately to the PC, or reveal its one-use
   code and paste that into FocusBridge on Windows. Confirm **Connect this PC**.
   The link/code expires after ten minutes and is bound to Windows. No new Windows
   password or Apple login is needed. Do not share it in a public issue or log.
3. Use a work app briefly, choose **Refresh recent apps**, then add the apps that
   should qualify as productive. Newly added rules apply from that moment onward.
4. Optional website earning: install the official ActivityWatch browser extension
   using the link in FocusBridge. Choose its local bucket and matching browser,
   save that source, and add productive website hostnames. Generic browser app time
   does not qualify; private browsing and unknown/ambiguous observations do not earn.

FocusBridge stays in the tray when you close its window. Enable **Start FocusBridge
when I sign in** if wanted. ActivityWatch has its own tray icon and local controls.

## Rewards

Under the current policy, four productive, non-idle minutes earn one distraction
minute on the same iPhone account. Activity settles for four minutes before upload,
then sync runs every 30 seconds. The first whole reward after starting a new work
interval therefore normally appears after about eight minutes, plus a sync tick.
Simply leaving the screen on is insufficient. Keep the bundled idle watcher's
default three-minute timeout. Mac and Windows activity at the same time counts once.

The iPhone's existing daily allowance, wellness rewards and seven-minute access
windows keep their normal behavior. This companion adds productive-work rewards;
it cannot spend the phone's balance.

Temporary network failures retain immutable queued work for retry. Work older than
the service's permitted upload window is archived locally without inventing credit.
If the PC connection is revoked, reconnect using a fresh Windows link from iPhone.

## Privacy and removal

ActivityWatch records apps, window titles, idle periods and configured browser
activity locally. FocusBridge sends configured rule identifiers and finalized work
intervals, not raw titles or full browsing URLs. Minimal technical reports contain
versions, status and error codes; repeated identical reports are throttled to
15 minutes. The connection screen explains this before you connect.

Credentials use current-user Windows DPAPI. FocusBridge settings and bounded queues
are in `%LOCALAPPDATA%\FocusBridge`. ActivityWatch owns a separate local database.
Quit both tray apps before uninstalling through Windows Settings → Apps. Uninstall
removes program files and the FocusBridge startup/protocol registration; local
accounting and ActivityWatch data are retained for you to manage separately.

[Privacy and support](https://github.com/akshat-gosain/FocusBridge-Downloads/blob/main/PRIVACY.md)
