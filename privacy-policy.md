---
title: Privacy Policy — SecretboxPlus
---

# Privacy Policy for SecretboxPlus

**Effective date:** 2026-11-23
**Last updated:** 2026-11-24

"SecretboxPlus" (the "App") is a paid Android app published by
Rastislav Hodul ("we", "us", or "the Developer"). It stores your
secrets in an encrypted vault on your device, protected by a password
that only you know. This privacy policy explains what data the App
handles, where that data goes, and your rights regarding it.

The short version: **the App collects nothing and sends nothing.** It
runs entirely on your device, has no network access, integrates no
third-party SDKs, and has no advertising. We never receive your
password or your secrets, so we cannot recover either of them for you.
Your data leaves the device only when you export an encrypted backup
yourself.

This version of the policy describes **SecretboxPlus 3.0.0 and later**.
SecretboxPlus is the successor to the earlier "Secret Box" and
"Secret Box+" apps; this policy does not cover those earlier apps.

---

## 1. What we collect

**Nothing through the App.** We do not collect, store, or transmit any
personal data, to ourselves or to anyone else, because the App has no
ability to transmit anything:

- The App declares **no `INTERNET` permission**. The Android platform
  therefore blocks every network operation it could attempt.
- The App contains **no analytics, telemetry, crash-reporting, or
  advertising SDKs**.
- We operate no server, and the App has no user accounts, sign-in, or
  cloud sync.

**Purchases.** The App is sold through Google Play, and Google handles
the purchase entirely. As the seller, we may receive limited order
information from Google Play, as Google's policies provide for sales
(for example, an order number, the country of purchase, and the
purchase status). We do not receive your payment card details. Google
processes your payment under the
[Google Privacy Policy](https://policies.google.com/privacy).

## 2. What is stored locally on your device

The App stores your **vault**: your compartments and the secrets inside
them (each with a title and a body). The vault is an encrypted database
in the App's private storage on your device, protected by your
password.

- Your password is never sent to us, and we have no way to recover it.
  If you forget it, we cannot unlock your vault for you.
- The App marks its screens as secure, so their contents are hidden
  from screenshots and from Android's recent-apps screen.

The vault is never sent anywhere by the App. It leaves the device only
in an encrypted backup file that you choose to export (see Section 4).

## 3. Android backup and device transfer

The App **opts out** of Android Auto-Backup and of Android's
device-to-device transfer. Your vault is therefore **not** included in
Google-account backups (Google Drive) and is not copied when you set up
a new phone from an old one.

This keeps your secrets out of third-party storage, but it has a
consequence: **if you uninstall the App, clear its data, or lose or
reset your device, the vault is deleted permanently**, and neither we
nor Google can restore it. To keep a backup, use the App's encrypted
export (Section 4) and store the file somewhere safe.

## 4. Encrypted backups, import, and the browser editor

### Exporting a backup

When you choose to, the App can export your vault as an encrypted
backup file (`.sbx`). You pick a separate backup password when you
export. The file is encrypted with a key derived from that password
(PBKDF2-HMAC-SHA256 and AES-256-GCM).

You decide where the file goes: you can save it to a location you pick,
or send it through Android's share sheet to an app of your choice (for
example, email or a cloud drive). The App exports only when you ask it
to. Once you hand the file to another app or service, that service's
own privacy policy applies to it.

All of your stored content (compartment names, secret titles, and
secret bodies) is encrypted inside the file. The file can still be
recognized as a SecretboxPlus backup, and its size roughly reflects how
much it contains. The protection depends on your backup password, so
**choose a strong one**. We cannot recover a forgotten backup password.

### Importing

You can import an old Secret Box database file or an `.sbx` backup by
picking it with Android's file picker. The App reads the file on your
device; nothing is uploaded.

### The browser editor

As an optional companion tool, a static web page lets you open, view,
and edit an `.sbx` backup on a computer. It runs **entirely inside your
browser**: your file and your backup password are never uploaded. The
page's content security policy forbids it from making network
connections, and the page asks your browser not to translate it
automatically (translation would send its text to a translation
service).

The editor is a set of static files. We offer a hosted copy at
<https://secretboxplus.rhodul.workers.dev>, served by Cloudflare. When
you load that page, Cloudflare (the host) may process standard
web-server data such as your IP address, under the
[Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/).
We receive none of that data, and the page never sends your file or
password anywhere: decryption and editing happen entirely in your
browser. You can also run the same files on your own computer without
any server.

This policy itself is hosted on GitHub Pages. As with any website,
GitHub may process standard web-server data such as your IP address when
you load it, under the
[GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

## 5. What we do NOT do

For the avoidance of doubt, SecretboxPlus does **not**:

- Require or offer user accounts or sign-in.
- Operate a server or any cloud sync.
- Run any analytics, telemetry, or crash reporting.
- Access the network at all — the App holds no `INTERNET` permission.
- Request dangerous permissions. It has no access to your camera,
  contacts, location, or microphone.
- Contain advertising or advertising identifiers.
- Send your password or your secrets to us or to anyone else.
- Sell or share your data with any third party.

## 6. Children

SecretboxPlus is **not directed at children under 13**. Because the
App collects no personal data from anyone, it collects none from
children.

## 7. Your rights

**Local data.** Uninstalling the App, or clearing its data in Android
Settings, permanently deletes your vault from the device. Because the
App is excluded from Android backups (Section 3), no copy remains in
your Google Account. Backup files you exported stay wherever you put
them until you delete them.

**Everything else.** The App sends us nothing, so the only information
we may hold about you is the limited Google Play order information
described in Section 1. To ask about that information or to request its
deletion, contact us (Section 10). Rights of access, correction,
erasure, portability, and objection under the GDPR, CCPA/CPRA, VCDPA,
and similar laws apply to that information. For everything else, they
are satisfied by the App's design: there is no other personal data
processing to exercise them against.

## 8. Data retention

**Local data:** retained on your device until you uninstall the App or
clear its data via Android Settings.

**Exported backups:** retained wherever you saved or sent them, under
your control and the policies of the service you chose.

**Purchase information:** order information that Google Play makes
available to us is held in Google Play Console, subject to Google's
retention practices.

**Everything else:** nothing is retained, because nothing is collected.

## 9. Changes to this policy

We may update this privacy policy from time to time to reflect changes
in the App or in applicable law. Changes take effect on the date posted
as "Last updated" at the top of this document, and a material change
(for example, adding network access or any data collection) will be
reflected in the Play Store listing's Data Safety section. Continued
use of the App after an update constitutes acceptance of the revised
policy.

Historical versions of this document are available in the
[public Git history](https://github.com/rhodul/secretboxplus-legal/commits/main/privacy-policy.md)
of its source repository.

## 10. Contact

For privacy questions specific to SecretboxPlus:

**Developer:** Rastislav Hodul
**Email:** rhodul@gmail.com

---

*SecretboxPlus is published by Rastislav Hodul. The App is distributed
via the Google Play Store under the package name
`com.gnugu.secretboxplus`. This document's source repository:
[github.com/rhodul/secretboxplus-legal](https://github.com/rhodul/secretboxplus-legal).*
