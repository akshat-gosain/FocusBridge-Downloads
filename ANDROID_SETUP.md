# FocusBridge for Android

Download the signed [Android APK](https://github.com/akshat-gosain/FocusBridge-Downloads/releases/download/android-v0.3.0/FocusBridge-Android-0.3.0.apk).
Android 10 or later is required. This is a direct APK download, not a Google Play listing.

1. Open the APK on your Android phone. Allow that browser/file manager to install
   this downloaded app if Android asks; keep other security protections enabled.
2. Open FocusBridge and create a username and password. Save the recovery code in
   a password manager. There is no email password reset. Returning users sign in
   to the same account rather than creating another account.
3. Follow **Usage Access**, **FocusBridge Accessibility**, and **Access-window
   notification** in the app. Android grants these in its own Settings screens.
   Some phones require **App info → menu → Allow restricted settings** for a
   personally installed APK before Accessibility can be enabled. This is an
   Android permission step, not a request to disable Play Protect.
4. Choose your distracting native apps. Adding an app applies immediately;
   requested removals wait until the next account day.
5. Choose **Apps and account → Connect Mac or Windows**. Install the matching
   desktop companion, create a private connection link for that computer, open
   it there and confirm Connect. Each computer needs its own link. A Mac, a
   Windows PC, or both can earn for the same phone. Overlapping productive
   intervals count once. Select productive apps in the desktop companion.

The account starts each day with **35 active minutes**, plus verified rewards.
Request access in FocusBridge, or open a protected app and tap its access button.
Each window lasts at most **seven elapsed minutes**. Only foreground use of
selected apps spends the daily balance; leaving them or locking the screen does
not spend the whole seven minutes. There is no fixed number of unlocks.
The visible access notification shows the remaining balance and window timer.
Its final-minute accent changes to red. Balance/rewards sync automatically.

## One phone, multiple computers

The service supports **one active spending phone per account**: Android or iPhone.
Adding a computer does not add another phone balance or disconnect the other
computer. Two phones cannot enroll concurrently against one account.

Replacing a phone requires a fresh account sign-in. If today's allowance was
already bound, replacement waits until the next account day so the old offline
phone cannot spend the same allowance twice. Revoking, reinstalling or resetting
a password does not create a new daily bank. Save your password/recovery code
before uninstalling. Android does not currently provide Sign in with Apple;
an Apple-only account needs a password identity linked by an authenticated owner
before it can sign in on Android. The current iPhone build 32 does not yet expose
that new credential-linking UI; self-service migration of an Apple-only account
is not included in this APK delivery. Do not make a second account expecting balances
or existing computer connections to merge automatically.

## Offline operation and Android limits

An already verified allowance can be used locally until its signed account-day
expiry, including during a temporary network outage. Pending usage is persisted
and retried with idempotency keys. No new account-day allowance is invented
offline. Restarting the phone or changing its clock requires a fresh sync before
another window. Keep automatic date/time enabled.

FocusBridge uses Android Usage Access and a package-only Accessibility service.
It does not retrieve screen text, messages, passwords or screenshots. The visible
foreground service runs during requested access windows. Android and manufacturer
battery controls can stop an app; force-stop, uninstalling or revoking protection
permissions can bypass this form of self-control protection. This APK does not
claim device-owner/parental tamper resistance.

This Android release protects **native apps**. Website-path/YouTube Shorts
filtering and Health Connect rewards are not implemented in this APK. Apple
Health remains an iPhone connector, not an Android feature.

## Verification status

Version **0.3.0 (1)** is release-signed. Server account, pairing, single-phone,
deduplication and reward tests; Android meter tests; signed-allowance rejection;
Room transaction/reopen tests; release compilation and lint are recorded with the
release. **Physical Android acceptance has not been run: no Android device was
available.** In particular, permission screens, OEM background behavior, shielding
over real apps and measured screen-on/screen-off use still need device verification.
Compilation and simulated framework checks are not a substitute for that test.

For an update, install a newer APK with the same application ID and signing
certificate over the existing installation. Uninstalling clears private local
state and Android Keystore credentials. Read [privacy](PRIVACY.md) and
[support](SUPPORT.md); never send passwords, recovery codes or private pair links.
