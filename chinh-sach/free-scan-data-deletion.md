---
title: "Data Deletion Request — ScanGo"
description: "How to delete your data from ScanGo: instant on-device deletion plus advertising-data controls for AdMob and Firebase Crashlytics."
keywords: ["data deletion", "ScanGo", "privacy", "AdMob opt-out", "AAID reset"]
slug: free-scan-data-deletion
canonical: "https://nextsmart.vn/chinh-sach/free-scan-data-deletion"
ogTitle: "Data Deletion — ScanGo"
ogDescription: "Delete your ScanGo data: documents, advertising ID, crash diagnostics. Step-by-step guide."
dateModified: "2026-05-19"
---

# Data Deletion Request — ScanGo

**App:** ScanGo (Vietnamese document scanner)
**Developer:** Nexttech Smart Solutions Company Limited
**Last updated:** 19/05/2026

ScanGo is an on-device document scanner. Most of your data never leaves your device, so deletion is immediate. This page explains how to delete each category of data ScanGo or its third-party SDKs hold.

---

## 1. Documents, OCR text, and app data (on-device)

**Stored on:** your device only (Android Internal Storage).
**Retention:** kept until you delete it.

**How to delete:**

- **Delete a single document** — Open ScanGo → long-press a document → choose **Delete**.
- **Delete all documents at once** — Open ScanGo → Settings → *(or)* uninstall the app. Uninstalling removes all scanned images, OCR text, folders, and settings immediately and irreversibly.
- **Clear app storage from system settings** — Android: Settings → Apps → ScanGo → Storage → **Clear storage**. This wipes everything including settings.

No data in this category is retained by Nexttech after deletion — we never had a copy to begin with.

---

## 2. Advertising data held by Google AdMob

**Stored by:** Google (not Nexttech). Governed by [Google's Privacy Policy](https://policies.google.com/privacy).
**What is held:** Advertising ID (AAID), approximate location from IP, device info, ad-interaction events.
**Retention:** controlled by Google's own retention schedule.

**How to delete or stop collection:**

- **Remove ads entirely** — Open ScanGo → Settings → **Buy Lifetime** (one-time purchase). After purchase, AdMob SDK is no longer invoked by ScanGo and stops collecting your Advertising ID for our app.
- **Reset your Advertising ID** — Android: Settings → Privacy → Ads → **Delete advertising ID** (or **Reset advertising ID**). This disconnects future ad events from past events.
- **Opt out of Ads Personalisation** — Android: Settings → Privacy → Ads → toggle **Opt out of Ads Personalisation**.
- **Request deletion directly from Google** — visit [myaccount.google.com](https://myaccount.google.com) → Data and privacy → My ad center, or contact Google via [policies.google.com](https://policies.google.com).

---

## 3. Crash diagnostics held by Firebase Crashlytics

**Stored by:** Google Firebase (not Nexttech directly, but accessible to us). Governed by [Firebase Data Processing Terms](https://firebase.google.com/terms/data-processing-terms).
**What is held:** anonymous stack traces, device model, OS version, app version. No document content. No personal identifiers.
**Retention:** Firebase Crashlytics retains crash reports for **90 days** by default.

**How to delete:**

- **Uninstall ScanGo** — once you uninstall, no new crash reports are sent. Existing reports age out within 90 days.
- **Request deletion of past reports** — email **contact@nextsmart.vn** with the subject line `Data Deletion Request — Crashlytics` and the approximate dates you used the app. We will issue a deletion request through the Firebase console. We respond within 30 days.

---

## 4. Purchase records held by Google Play Billing

**Stored by:** Google Play.
**What is held:** purchase token for Lifetime Unlock (only if you bought it).
**Retention:** controlled by Google Play.

**How to request deletion:** purchase records are part of your Google account billing history. Contact Google Play support at [support.google.com/googleplay](https://support.google.com/googleplay).

---

## 5. Summary table

| Data category | Location | How to delete | Time to take effect |
|---|---|---|---|
| Scanned documents, OCR text, settings | Your device | Uninstall app OR delete in-app | Immediate |
| Advertising ID, ad events | Google AdMob | Buy Lifetime Unlock + reset AAID | Immediate (for app) |
| Crash diagnostics | Firebase Crashlytics | Uninstall + email us | Up to 30 days |
| Purchase token | Google Play | Contact Google Play | Per Google policy |

---

## 6. Contact for deletion requests

For any request not covered above — or to request confirmation that crash reports have been deleted — email:

**contact@nextsmart.vn**

Subject line: `Data Deletion Request — ScanGo`

Please include:
- The approximate dates you used ScanGo
- The device model and Android version (helps us locate the right diagnostic records)
- Whether you also want your Lifetime Unlock entitlement removed (purchase refund requests go through Google Play, not us)

We respond to all data deletion requests within **30 calendar days**, as required by applicable data protection law.

---

**Developer:** Nexttech Smart Solutions Company Limited
**Website:** [nextsmart.vn](https://nextsmart.vn)
