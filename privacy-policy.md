# QRsuite — Privacy Policy

**Effective date:** April 19, 2026

This policy explains what data QRsuite collects, why, and the choices you have. It is written in plain English on purpose — you should be able to read it in a few minutes.

---

## 1. Who we are

QRsuite is an iOS app for scanning and generating QR codes and barcodes. It is developed and operated by **Abdullah Al Hadi** ("we", "us"). For any privacy questions, contact us at **hadi.fiftytwo@gmail.com**.

This policy covers the QRsuite iOS app and its bundled extensions (Widget and Share Extension).

---

## 2. Data we collect

### Stays only on your device — never sent anywhere

Everything below is stored locally in the app using Apple's SwiftData framework. It lives on your device (and, if you enable it, in your private iCloud backup). We have no access to any of it.

- **Scan history** — every QR or barcode you scan, including the decoded text, timestamp, and any folder, note, or favorite flag you attach to it.
- **Created QRs** — QRs you generate, with their design settings and thumbnails.
- **Saved templates** — designs you save to reuse later.
- **Folders and notes** — organizational data you add yourself.
- **Preferences** — your settings (theme, App Lock on/off, etc.), stored in iOS user defaults.

You can delete any of this at any time from within the app (swipe-to-delete, bulk-delete, or Settings → "Clear all history"). Uninstalling the app removes all of it.

### Sent to Firebase (Google)

We use two Firebase services from Google to improve the app: **Analytics** and **Crashlytics**. Both are configured with the minimum data surface needed for product decisions and crash fixing — no advertising identifiers, no cross-app tracking.

**Firebase Analytics** collects:

- Device identifiers that are scoped to this app only (Apple's IDFV, a Firebase installation ID). These cannot identify you across other apps.
- Device type, OS version, app version, language, country (derived from IP).
- A record of which screens you view.
- The following specific events, so we can see which features people actually use and decide what to keep, fix, or cut:

  | Event | What it means |
  |---|---|
  | `qr_scanned` | A scan succeeded. Includes the type of code (url/wifi/text/etc) and the source (camera/gallery). Does **not** include the scanned text. |
  | `qr_created` | A QR was generated. Includes the kind (url/wifi/etc). Does **not** include the payload. |
  | `qr_shared` | A QR was shared. Includes kind and destination (system share / HD PNG / PDF). |
  | `qr_saved` | A QR was saved to "My QRs". Includes kind. |
  | `scan_failed` | A scan attempt failed. Includes the source and failure reason. |
  | `scan_action` | A post-scan action (Open URL, Call, Copy password, Add to Contacts, etc.). Action name only — no payload. |
  | `pro_gate_bounced` | A Pro-only feature was tapped without a Pro subscription. Feature name only. |
  | `pro_upgrade_tapped` | The Pro upgrade button was tapped. Plan name (lifetime/yearly/monthly) only. |
  | `template_used` | A saved template was applied. Template's random ID only — no name. |
  | `template_created` | A new template was saved. Random ID only. |
  | `history_opened` | The History tab was opened. |
  | `history_item_deleted` | An item was deleted from history. Item kind only (scanned/created). |
  | `history_item_shared` | A history item was shared. Item kind and destination. |
  | `history_item_reused` | A created QR was reused in Create. |
  | `history_item_pinned` | A QR was pinned or unpinned from the widget. |
  | `history_item_noted` | A note was added, changed, or cleared on a history item. Note text is **not** included. |
  | `folder_created` | A folder was created. Name is **not** included. |
  | `folder_renamed` | A folder was renamed. |
  | `folder_deleted` | A folder was deleted. |
  | `settings_changed` | A preference changed (App Lock, appearance theme). Setting name and new value only. |
  | `history_cleared` | The "Clear all history" action was used. Total count only. |
  | `app_lock_triggered` | The biometric unlock prompt was shown. |
  | `screen_view` | Automatic — fires each time you open a screen in the app. |

**What we do NOT send:** the contents of any QR or barcode (scanned or created), the text of your notes, the names of your folders or templates, the contents of your photo library, any image bytes, any passwords, or any Wi-Fi credentials.

**Firebase Crashlytics** collects data only when the app crashes:

- Stack traces from the crash.
- A snapshot of device state at the time of the crash (OS version, device model, memory pressure, etc.).
- Breadcrumbs — short text messages we log as you use the app (e.g. "opened Design screen") to help us reproduce the crash. These never contain QR payloads, notes, or personal content.
- Non-fatal errors explicitly reported by the app (e.g. "QR render failed").

---

## 3. Permissions the app asks for

- **Camera** — required to scan codes in real time. Frames are processed on-device by Apple's Vision framework. Camera frames are never stored and never transmitted.
- **Photo Library** — optional. Used only when you tap the gallery picker to scan a photo. We read only the image(s) you explicitly select. Nothing is uploaded.
- **Face ID / Touch ID / passcode** — optional, only used when App Lock is enabled. The check happens locally via Apple's LocalAuthentication framework. Your biometric data never leaves your device and is never seen by the app.

---

## 4. How we use this data

- **Local data** (scan history, templates, etc.) powers the app's features for you — searching your own history, reusing a created QR, etc. It is not used for anything else.
- **Firebase Analytics** tells us which features are actually being used. We look at aggregate counts — not at individual users. The goal is to decide what to improve and what to remove.
- **Firebase Crashlytics** tells us when and why the app crashes so we can fix the underlying bug.

We do not sell your data. We do not share it with advertisers. We do not use it to build profiles across other apps.

---

## 5. Third parties

The only third-party service the app communicates with is **Firebase**, operated by Google LLC. Google processes Analytics and Crashlytics data as our service provider, under the [Firebase Data Processing Terms](https://firebase.google.com/terms/data-processing-terms). Google's own privacy practices are covered by the [Google Privacy Policy](https://policies.google.com/privacy).

No other third-party analytics, advertising, or tracking SDK is bundled in the app.

---

## 6. How long we keep it

- **Local data** — kept on your device until you delete it or uninstall the app.
- **Firebase Analytics** — Google retains event-level data for **14 months** (Firebase's default), after which older events are aggregated or dropped.
- **Firebase Crashlytics** — Google retains crash reports for **90 days**.

---

## 7. Your rights and choices

- **Delete your history** at any time — swipe-to-delete, bulk-delete, or **Settings → Clear all history**.
- **Turn off analytics system-wide** — iOS **Settings → Privacy & Security → Analytics & Improvements → Share iPhone Analytics**. When this is off, Firebase still receives minimal crash data; you can prevent even that by uninstalling the app.
- **Access or erase your data** under GDPR (EEA, UK), CCPA/CPRA (California), or similar laws — email **hadi.fiftytwo@gmail.com**. Because we don't tie analytics data to a persistent identity, the most reliable erasure is uninstalling the app, which invalidates the Firebase installation ID.
- **Opt out of analytics inside the app** — not currently available as a per-app toggle. If you'd like one, email us and we'll prioritize it.

---

## 8. Children's privacy

QRsuite is not directed at children under 13. We don't knowingly collect data from children under 13. If you believe a child has used the app and want the data associated with that device erased, email **hadi.fiftytwo@gmail.com** — we'll help you uninstall and reset.

---

## 9. Security

- Local data is stored using iOS's standard app sandbox protections. If you enable App Lock, it's additionally gated behind Face ID / Touch ID / passcode.
- Data sent to Firebase travels over HTTPS (TLS).
- We cannot guarantee perfect security — no one can. If we become aware of a breach that affects your data, we will notify you as required by applicable law.

---

## 10. Changes to this policy

If we change this policy, the new version will replace this page at **https://hadicuet.github.io/qrsuite-legal/** and the "Effective date" at the top will be updated. Material changes (e.g. a new third-party service, a new category of data) will be called out in the app's release notes.

---

## 11. Contact us

Questions, requests, or complaints: **hadi.fiftytwo@gmail.com**.
