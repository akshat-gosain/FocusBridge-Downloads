# FocusBridge Privacy Notice

Updated November 27, 2026. Applies to the FocusBridge iPhone and Android apps, Mac and Windows
companions, Safari extensions and associated FocusBridge account service.

FocusBridge is operated by Akshat Gosain. For privacy requests or support, contact
[akshat.gosain1990@gmail.com](mailto:akshat.gosain1990@gmail.com). Do not include
passwords, pairing codes, Apple tokens or raw Health records in a support message.

## What FocusBridge Does

FocusBridge is a personal focus and device-management tool. It combines a daily
distraction allowance with rewards from productive computer activity and, optionally,
Apple Health Move-goal progress. It measures use of selected distractions to
reconcile your balance. It is not a service for supervising other adults or employees.

## Account And Required Service Data

Starting with iPhone build 33, Screen Time setup is available without registering
or signing in. Your permission and app/site selections are managed locally.
To provide the daily balance and Live Activity updates without sign-in, the app
uses a random device-session identifier and a secure installation credential
stored in Keychain. The service stores the credential's hash, timezone, app version
and the balance/usage records described below, under an internal device profile.
It does not request a name, email, Apple identity or password for this mode.
Device-only service records are pseudonymous, not anonymous aggregate data.
An internet connection is needed to initialize or renew a signed daily balance;
already issued valid balances continue to support local enforcement offline.
Optional Apple sign-in can link the same profile for recovery and computer
pairing without resetting its balance. Accounts with different identities are
not automatically merged.

When you use native Sign in with Apple, FocusBridge receives and verifies Apple's
app-specific account identifier, identity token and one-time authorization code.
The app does not request your Apple account password, name or email through that
sign-in. Apple's own services handle the Apple account authentication.

Android supports a FocusBridge username/password account. The server stores the
normalized username, an Argon2id password hash and a hash of a one-time recovery
code, not the plaintext password or recovery code. Password verification is rate
limited and memory-intensive work is bounded. Password recovery rotates the code
and revokes device connections; there is no email recovery. An authenticated owner
can link this identity to an existing account. Signing in does not merge accounts.

The service stores an encrypted Apple refresh grant so it can revoke your Apple
authorization when you delete your account. Device/setup/pairing credentials are
stored as hashes on the server. Device credentials use native Keychain on Apple
devices, Android Keystore-backed AES-GCM on Android and current-user Windows DPAPI on Windows; temporary setup and one-use
pairing links must be kept private.

Required service records include account and installation identifiers, your chosen
device name, platform/version, account timezone, pairing/revocation status, productive
app rules, eligible-work intervals, daily rewards, access-window and selected-usage
totals, balance revisions and reconciliation receipts. These records are linked to
your account and are used to provide the service, prevent duplicate rewards and
reconcile usage. Account syncing is separate from optional diagnostics.

Apple's opaque iPhone app/site selection tokens stay on your device. FocusBridge
syncs a selection identifier and measured usage totals, not those selection tokens.
Your iPhone needs your explicit Screen Time authorization to apply protection.

On Android, selected package names, native Usage Access events and package-only
Accessibility changes are processed on the phone to shield selected apps and
measure active use. These package names/events are not uploaded as diagnostics.
Android does not retrieve accessibility screen content, text, messages, passwords
or screenshots. Account-day usage totals, signed allowance bindings and bounded
technical status/error reports sync to the service. There is no Android Health
Connect collection in this release. Android app backups are disabled and exclude
credentials and accounting state.

## ActivityWatch On Your Computer

The Mac and Windows installers include the official, unmodified ActivityWatch application.
ActivityWatch is a separate open-source app with its own local database and controls.
Depending on the watchers you enable, it can record active-window titles, application
names, idle/active periods and browser activity locally on your computer.

FocusBridge evaluates eligible work locally against your productive rules and idle
periods. Work uploads contain rule identifiers and interval timestamps/durations,
not raw window titles or full browser URLs from ActivityWatch. Productive app names
or website rules you configure are part of your account policy.

Deleting FocusBridge's account does not remove the separate ActivityWatch database.
Manage or remove that local data using ActivityWatch's controls. See
[ActivityWatch's privacy documentation](https://docs.activitywatch.net/en/latest/privacy.html)
and the accompanying third-party notices.

## Optional Apple Health Connection

Apple Health access is optional and uses a separate in-app disclosure and Apple's
read-permission prompt. FocusBridge reads the current day's Move activity and goal
to calculate reward milestones. It does not write Health records.

Raw activity and goal values stay on your iPhone in protected local wellness storage
excluded from app backups. Only completed reward milestones, their account day,
provider, observation time, an opaque daily goal identifier and resulting reward
receipts are sent to the account service. These derived milestones are still
Health/Fitness-related data linked to your account; they are not anonymous.

Disconnecting Apple Health stops future reads/uploads and clears pending local
wellness uploads. Previously credited rewards remain. A fixed daily reward goal
may remain locally until the next daily update to prevent duplicate rewards.
You can also manage Health permissions in Apple's Health app. Deleting the
FocusBridge account does not delete your underlying Apple Health records.

## Live Activities And Apple Services

Live Activity tokens, the push environment, window deadline and balance/display
state are processed by FocusBridge and Apple's push-notification infrastructure
to update your activity. Your displayed balance can be visible on the Lock Screen
or Dynamic Island. iOS controls permission and background delivery.

Apple also processes TestFlight distribution and native sign-in. The first release
has no configured paid product, does not send purchase history, and requires no
purchase or subscription. Apple has its own privacy policies.

## Limited Technical Reports

Starting with iPhone build 30, a one-time privacy notice explains limited operational
reports before collection begins. Tapping Agree and continue gives consent to this
reporting. Reports are then sent automatically to identify setup and protection
failures; there is no separate operational-report toggle. They include app/build and OS versions,
process component and random session/event identifiers, error codes/domains,
Screen Time authorization results, and selection counts and setup save outcomes.
They are linked to your account and device, not anonymous. They exclude selected
app names, selection tokens, free-text error messages, usage/balance values, access
window identifiers and raw Health data. Identical reports are limited to once per
minute per process, with a bounded local queue; offline reports are retried after
device enrollment and connectivity resume. Delivery is not guaranteed if the app
cannot run or the device has not enrolled. Detailed support traces remain separately
optional; their existing opt-out is not changed by the operational-report channel.

The Windows connection screen explains its limited operational reporting before
you choose Connect. Windows reports include app/OS versions, random session/event
identifiers, a fixed connection/sync state and technical error codes. They exclude
raw activity, app names, URLs, free-text error messages, balances and Health values.
Repeated identical reports are limited to once per 15 minutes per state/error;
the local retry queue is bounded to 100 events. A separate bounded local log records
operation names and error types/codes. The ActivityWatch database is independent
of these reports and remains local.

## Android Operational Reports And Optional Feature Feedback

On Android 0.3.1 and later, required limited operational reports additionally
include a random installation/support reference; setup/permission states and
counts; request identifiers, timing, route templates and fixed error codes;
window timing and usage/balance totals; own-code crash method/line frames and a
fingerprint; and available OS-reported process-exit/ANR reason codes. A suspected
foreground UI stall can also be reported. Exception messages, raw stack/ANR dumps,
request bodies, passwords and selected app names are excluded. Limited setup
reports can arrive before an account is created or a device is enrolled, subject
to strict field, size and admission limits. The reference can correlate those
technical reports with later account-linked reports. It is not a login secret.

The Android local technical journal is separate from protection/accounting data,
capped at 128 events/192 KiB and seven days, with daily category quotas and
duplicate suppression. A fatal Java error leaves a small private technical marker
for the next launch. Android 11+ may supply prior own-process exit reasons; raw
native crash/ANR trace streams are not read/uploaded. Reports may require reopening
and connectivity to upload and are not a continuous screen or activity recording.

Android's optional feature feedback contains a feature category, rating and a
predefined issue category, linked to the account/device when sent. There is no
free-text feedback capture. Automatic prompts can be skipped or stopped; the
feature can be disabled independently of operational reports and protection.
Unsent local reports/support reference are cleared/rotated on account deletion;
unlinked pre-login reports expire under the seven-day service policy.

## Optional Detailed Diagnostics

The separate iPhone detailed-support option defaults off for new installations.
You can change it in Settings; Android's operational reports above do not use this toggle.
The owner's earlier private test installations may retain their existing choice.

When enabled, diagnostics can include app/OS version, process and session identifiers,
errors, permission/protection events, counts, elapsed request/responsiveness timings,
usage/balance revisions and access-window correlation identifiers. These records
are linked to your account/device. FocusBridge filters diagnostic fields and redacts
recognized credentials and URLs. The release candidate excludes raw system boot
uptime and website hostnames from diagnostic uploads; it does not upload raw Health
activity or goal values in diagnostics.

Turning detailed logs off clears that local queue and stops later detailed batches.
It cannot recall an in-flight request or immediately erase received events.
Limited operational reports and required account, reward and balance traffic continue.

## Retention And Account Deletion

Account, device, policy, accounting and reward records are retained to operate your
active account; they do not currently have a general short age-based expiry.
Android operational, pre-login and feedback reports use a rolling seven-day
retention policy with bounded indexed cleanup. Other platforms retain ordinary
diagnostic traces/samples for up to 48 hours and errors/selected lifecycle events
for up to 14 days. These cleanup policies do not erase account balances or rewards.

Separate operational server logs are limited by size-based rotation. They can include
request/device identifiers, route, error/status and timing information. They are not
used for advertising. Encrypted routine database backups rotate after 14 days;
deleted data can remain in those backups until expiry. Service signing/encryption
keys and operational source/configuration recovery archives are stored separately.
New routine business backups omit transient diagnostic-table data while retaining
their schemas; earlier backups containing diagnostics expire under the existing
fourteen-day policy.

Use Settings > Delete account in the iPhone app, with fresh Apple authentication
when required. The service revokes Apple authorization before removing account-scoped
device credentials, policies, accounting, reward, wellness and diagnostic records.
If revocation fails, the app reports an error rather than claiming deletion succeeded.
Minimal random account identifiers and a deletion record can remain to identify the
deleted account without retaining its Apple sign-in identity or account history.
Contact support if you cannot complete deletion in the app.

For a device-only profile that has not been linked to Apple, use Settings >
Delete device data. This removes its service records and revokes the installation
credential without requiring Apple sign-in. Deletion needs an internet connection;
the app reports an error if service-side deletion cannot be confirmed.

Local records on your own devices, the independent ActivityWatch database and Apple
Health records are subject to their separate controls. Uninstalling an app alone
does not request server account deletion, and Keychain credentials may survive an
app reinstall.

## Recipients And Security

Data required for the account service is processed on FocusBridge's hosted service
and its infrastructure. Apple processes the Apple services described above. GitHub
hosts public download/support materials; visiting GitHub is subject to GitHub's
own data handling. Sending a support email shares the information you include with
the operator and the email provider. Data may be processed outside your country.

FocusBridge does not sell your data, use Health or device-usage data for advertising,
share it with data brokers, or configure cross-company advertising tracking.
Access to Health, Screen Time, Accessibility and Safari extensions remains under
your platform's permission controls.

The service uses HTTPS, native Keychain or Windows DPAPI for device credentials, hashed server-side
credentials, encrypted Apple refresh grants and encrypted database backups. These
safeguards do not mean every database field is encrypted individually, nor can any
software promise perfect security or uninterrupted iOS background delivery.

For access, correction, deletion or other privacy questions, use the contact above.
This notice will be updated when the actual data handling changes.
