# FocusBridge Privacy Notice

Updated November 21, 2026. Applies to the FocusBridge iPhone app, Mac companion,
Safari extensions and associated FocusBridge account service.

FocusBridge is operated by Akshat Gosain. For privacy requests or support, contact
[akshat.gosain1990@gmail.com](mailto:akshat.gosain1990@gmail.com). Do not include
passwords, pairing codes, Apple tokens or raw Health records in a support message.

## What FocusBridge Does

FocusBridge is a personal focus and device-management tool. It combines a daily
distraction allowance with rewards from productive Mac activity and, optionally,
Apple Health Move-goal progress. It measures use of selected distractions to
reconcile your balance. It is not a service for supervising other adults or employees.

## Account And Required Service Data

When you use native Sign in with Apple, FocusBridge receives and verifies Apple's
app-specific account identifier, identity token and one-time authorization code.
The app does not request your Apple account password, name or email through that
sign-in. Apple's own services handle the Apple account authentication.

The service stores an encrypted Apple refresh grant so it can revoke your Apple
authorization when you delete your account. Device/setup/pairing credentials are
stored as hashes on the server. Device credentials are stored in native Keychain
on your devices; temporary setup and one-use pairing links must be kept private.

Required service records include account and installation identifiers, your chosen
device name, platform/version, account timezone, pairing/revocation status, productive
app rules, eligible-work intervals, daily rewards, access-window and selected-usage
totals, balance revisions and reconciliation receipts. These records are linked to
your account and are used to provide the service, prevent duplicate rewards and
reconcile usage. Account syncing is separate from optional diagnostics.

Apple's opaque iPhone app/site selection tokens stay on your device. FocusBridge
syncs a selection identifier and measured usage totals, not those selection tokens.
Your iPhone needs your explicit Screen Time authorization to apply protection.

## ActivityWatch On Mac

The Mac installer includes the official, unmodified ActivityWatch application.
ActivityWatch is a separate open-source app with its own local database and controls.
Depending on the watchers you enable, it can record active-window titles, application
names, idle/active periods and browser activity locally on your Mac.

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

## Optional Diagnostics

New installations default optional diagnostics off. You can change this in Settings.
The owner's earlier private test installations may retain their existing choice.

When enabled, diagnostics can include app/OS version, process and session identifiers,
errors, permission/protection events, counts, elapsed request/responsiveness timings,
usage/balance revisions and access-window correlation identifiers. These records
are linked to your account/device. FocusBridge filters diagnostic fields and redacts
recognized credentials and URLs. The release candidate excludes raw system boot
uptime and website hostnames from diagnostic uploads; it does not upload raw Health
activity or goal values in diagnostics.

Turning diagnostics off clears the queued local diagnostic events and stops later
batches. It cannot recall an in-flight request or immediately erase events already
received by the service. Required account, reward and balance traffic continues.

## Retention And Account Deletion

Account, device, policy, accounting and reward records are retained to operate your
active account; they do not currently have a general short age-based expiry.
Ordinary stored diagnostic traces/samples are retained for up to 48 hours; errors
and selected lifecycle events for up to 14 days, with bounded periodic cleanup.

Separate operational server logs are limited by size-based rotation. They can include
request/device identifiers, route, error/status and timing information. They are not
used for advertising. Encrypted routine database backups rotate after 14 days;
deleted data can remain in those backups until expiry. Service signing/encryption
keys and operational source/configuration recovery archives are stored separately.

Use Settings > Delete account in the iPhone app, with fresh Apple authentication
when required. The service revokes Apple authorization before removing account-scoped
device credentials, policies, accounting, reward, wellness and diagnostic records.
If revocation fails, the app reports an error rather than claiming deletion succeeded.
Minimal random account identifiers and a deletion record can remain to identify the
deleted account without retaining its Apple sign-in identity or account history.
Contact support if you cannot complete deletion in the app.

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

The service uses HTTPS, native Keychain for device credentials, hashed server-side
credentials, encrypted Apple refresh grants and encrypted database backups. These
safeguards do not mean every database field is encrypted individually, nor can any
software promise perfect security or uninterrupted iOS background delivery.

For access, correction, deletion or other privacy questions, use the contact above.
This notice will be updated when the actual data handling changes.
