# QRsuite — Privacy Policy

**Effective date:** October 29, 2026

This policy explains what data QRsuite collects, why, and the choices you have. It is written in plain English on purpose — you should be able to read it in a few minutes.

---

## 1. Who we are

QRsuite is an iOS app for scanning and generating QR codes and barcodes, and printing labels. It is developed and operated by **Abdullah Al Hadi** ("we", "us"). For the purposes of the EU / UK / EEA General Data Protection Regulation (GDPR) and the California Consumer Privacy Act (CCPA/CPRA), Abdullah Al Hadi is the **data controller** for personal data collected through the QRsuite app. For any privacy questions, contact us at **hadi.fiftytwo@gmail.com**.

This policy covers the QRsuite iOS app and its bundled extensions (Widget and Share Extension).

---

## 2. Data we collect

### Stored on your device

Everything below is stored locally on your device using Apple's SwiftData framework. By default none of it leaves your device, and we cannot see it.

- **Scan history** — every QR or barcode you scan, including the decoded text, timestamp, scan count, and any folder, note, or favorite flag you attach to it. You can pause saving new scans in Settings.
- **Created QRs** — QRs and barcodes you generate, with their design settings and thumbnails.
- **Saved templates, saved batches, label sheets and Brand Kit** — designs, label runs, sheets and brand colors and logo you save to reuse later.
- **Folders and notes** — organizational data you add yourself.
- **Preferences** — your settings (theme, App Lock on/off, label defaults, etc.), stored in iOS user defaults.

You can delete any of this at any time from within the app: swipe-to-delete, **Settings → Clear scan history**, or **Settings → Delete all data**, which removes everything listed here except your settings (theme, App Lock, scan settings and the like), including your iCloud copy. Uninstalling the app removes the local copy. If you have iCloud Backup enabled on your iPhone, Apple includes the app's data in your encrypted iCloud backup — that backup is between you and Apple.

### Sent to iCloud, only if you turn on iCloud Sync

iCloud Sync is an optional Pro feature and is off until you turn it on in Settings. When it is on, your scan history, created QRs, folders, notes and saved templates are also stored in your **private iCloud (Apple CloudKit) database**, tied to your Apple Account, so they stay in sync across your devices. That data is held and protected by Apple; we do not receive it and cannot access it. Turning sync off stops further uploads. **Settings → Delete all data** also deletes the iCloud copy.

### Backup files

**Settings → Back up everything** creates one file with your data. It is saved or shared only where you choose to send it; we never receive it.

### Sent to Firebase (Google)

We use three Firebase services from Google: **Analytics**, **Crashlytics** and **Remote Config**. They are always on in this version of the app; there is no in-app switch to turn them off. They are configured with the minimum data surface needed for product decisions and crash fixing — no advertising identifiers, no cross-app tracking.

**Firebase Analytics** collects:

- Device identifiers scoped to this app only (Apple's IDFV, a Firebase installation ID). These cannot identify you across other apps.
- Device type, OS version, app version, language, and country (derived from IP).
- Which screens you view in the app.
- Aggregate feature usage, so we can decide what to keep, fix, or cut:
  - The *type* of code you scan or create (URL, Wi-Fi, text, etc.) — never the content
  - Actions you take on a scan result (open, copy, share, add to contacts, etc.) — action name only
  - Which Pro-only features you attempt and which subscription plan you consider
  - Purchases you make in the app: the product, its price and currency, and whether it is a subscription. Apple handles the payment; we never see your payment details or your Apple Account
  - Your current plan (free, monthly, yearly or lifetime)
  - The choices you make during onboarding, and which Siri or Shortcuts actions you run — the option or action name only
  - Counts of operations on history, folders, templates, and notes (created, edited, deleted) — never the names or contents
  - Which settings you change (for example App Lock or iCloud Sync on or off) — the setting name and its new value only
  - Whether a scan or render attempt failed, with a generic reason (e.g. "no barcode found")

**We do NOT request App Tracking Transparency permission.** Firebase Analytics, as we use it, does not collect your advertising identifier (IDFA) and cannot link you across other apps or websites.

**What we do NOT send to Firebase:** the contents of any QR or barcode (scanned or created), the text of your notes, the names of your folders or templates, the contents of your photo library, any image bytes, any passwords, or any Wi-Fi credentials.

**Firebase Remote Config** lets us change a few app settings without an update, such as whether the one-time lifetime offer is shown and how long it lasts. To fetch them, the app sends its Firebase installation ID, app version and your device's language and region. It sends no usage data.

**Firebase Crashlytics** collects data only when the app crashes:

- Stack traces from the crash.
- A snapshot of device state at the time of the crash (OS version, device model, memory pressure, etc.).
- Breadcrumbs — short text messages we log as you use the app (e.g. "opened Design screen") to help us reproduce the crash. These never contain QR payloads, notes, or personal content.
- Non-fatal errors explicitly reported by the app (e.g. "QR render failed").

### Sent to Open Food Facts, only when you tap "Look up product"

On a scanned retail barcode (EAN or UPC) you can tap **Look up product**. Only then, QRsuite sends that barcode number to **Open Food Facts** (openfoodfacts.org), a community product database, and shows what it returns. Like any web request, this also reveals your **IP address** to Open Food Facts. The lookup is never automatic, never runs for batch scans or history, and we do not store the result. Open Food Facts handles the request under its own [privacy policy](https://world.openfoodfacts.org/privacy).
---

## 3. Permissions the app asks for

- **Camera** — required to scan codes in real time. Frames are processed on-device by Apple's Vision framework. Camera frames are never stored and never transmitted.
- **Photo Library** — optional. Used only when you tap the gallery picker to scan a photo, or to save a code you created. We read only the image(s) you explicitly select. Nothing is uploaded.
- **Face ID / Touch ID / passcode** — optional, only used when App Lock is enabled. The check happens locally via Apple's LocalAuthentication framework. Your biometric data never leaves your device and is never seen by the app.
- **Location** — optional, only when you create a Location QR. It fills in the coordinates of that code on your device.
- **Contacts and Calendar** — optional, only to add a scanned contact or event when you choose to save it.
---

## 4. How we use this data

- **Local data** (scan history, templates, etc.) powers the app's features for you — searching your own history, reusing a created QR, etc. It is not used for anything else.
- **Firebase Analytics** tells us which features are actually being used. We look at aggregate counts — not at individual users. The goal is to decide what to improve and what to remove.
- **Firebase Crashlytics** tells us when and why the app crashes so we can fix the underlying bug.
- **Firebase Remote Config** delivers app settings, such as whether the lifetime offer is on.

We do not sell your personal information, and we do not share it for cross-context behavioral advertising (as those terms are defined under the California Consumer Privacy Act). We do not share data with advertisers, and we do not build profiles across other apps.

---

## 5. Third parties

The services the app communicates with are:

- **Firebase**, operated by Google LLC — Analytics, Crashlytics and Remote Config, as described above. Google processes this data as our service provider, under the [Firebase Data Processing and Security Terms](https://firebase.google.com/terms/data-processing-terms). Google's own privacy practices are covered by the [Google Privacy Policy](https://policies.google.com/privacy).
- **Apple** — App Store purchases and subscriptions (we never see your payment details), and iCloud (CloudKit) if you turn on iCloud Sync. Apple's practices are covered by the [Apple Privacy Policy](https://www.apple.com/legal/privacy/).
- **Open Food Facts** — only when you tap **Look up product**, as described above.

Google primarily processes Firebase data on servers located in the **United States**. For users in the EEA, UK, or Switzerland, international transfers rely on Google's Data Processing and Security Terms, which incorporate the European Commission's Standard Contractual Clauses and the UK International Data Transfer Addendum.

No other third-party analytics, advertising, or tracking SDK is bundled in the app.
---

## 6. How long we keep it

- **Local data** — kept on your device until you delete it or uninstall the app.
- **iCloud copy** — kept in your private iCloud until you delete it with **Settings → Delete all data** or remove it in iOS Settings → your name → iCloud → Manage Storage.
- **Firebase Analytics** — Google retains event-level data for **14 months** (Firebase's default), after which older events are aggregated or dropped.
- **Firebase Crashlytics** — Google retains crash reports for **90 days**.
- **Open Food Facts** — we keep nothing; the request is handled by Open Food Facts under its own policy.
---

## 7. Your rights and choices

- **Delete your data** at any time — swipe-to-delete, **Settings → Clear scan history**, or **Settings → Delete all data**, which also deletes your iCloud copy.
- **Take your data with you** — **Settings → Back up everything** exports it to one file, and **Export history as CSV** (Pro) exports your scans and created codes.
- **Analytics and crash reports** — they are always on and there is no in-app switch. The iPhone **Analytics & Improvements → Share iPhone Analytics** setting in iOS does **not** control them. You can stop them by uninstalling the app, which also invalidates the Firebase installation ID.
- **Access or erase your data** under GDPR (EEA, UK), CCPA/CPRA (California), or similar laws — email **hadi.fiftytwo@gmail.com**. Because we don't tie analytics data to a persistent identity, the most reliable erasure is uninstalling the app.
- **Lodge a complaint** — if you're in the EEA, UK, or Switzerland and believe we're mishandling your data, you have the right to complain to your local data protection authority. We'd appreciate the chance to address your concern first — email **hadi.fiftytwo@gmail.com** and we'll respond within 30 days.
---

## 8. Children's privacy

QRsuite is not directed at children under 13. We don't knowingly collect data from children under 13. If you believe a child has used the app and want the data associated with that device erased, email **hadi.fiftytwo@gmail.com** — we'll help you uninstall and reset.

---

## 9. Security

- Local data is stored using iOS's standard app sandbox protections. If you enable App Lock, it's additionally gated behind Face ID / Touch ID / passcode, and the lock covers the whole app, including the app switcher.
- Data sent to Firebase and Open Food Facts travels over HTTPS (TLS). iCloud data is protected by Apple.
- We cannot guarantee perfect security — no one can. If we become aware of a breach that affects your data, we will notify you as required by applicable law.
---

## 10. Changes to this policy

If we change this policy, the new version will replace this page at **https://hadicuet.github.io/qrsuite-legal/** and the "Effective date" at the top will be updated. Material changes (e.g. a new third-party service, a new category of data) will be called out in the app's release notes.

---

## 11. Contact us

Questions, requests, or complaints: **hadi.fiftytwo@gmail.com**.
