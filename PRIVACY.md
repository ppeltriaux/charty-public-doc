# Privacy Policy

**Charty** is published by Pascal Peltriaux.

**Effective date:** 17 May 2026

---

## TL;DR

Charty doesn't collect anything. No accounts. No analytics. No ads. No third-party SDKs. Your data stays on your device.

---

## What data is collected

**None.** Charty does not collect, store, or transmit any personal data, usage analytics, or device identifiers to any server.

Specifically, Charty does **not**:

- Create user accounts
- Track usage, behaviour, or interactions
- Display ads
- Use third-party analytics SDKs (Google Analytics, Firebase, Mixpanel, etc.)
- Include any tracking pixels
- Make any network requests for telemetry, crash reporting, or "phone-home" purposes
- Sell, trade, or share data with any party (because there is no data to share)

This is enforced by Apple's iOS sandbox + the absence of any networking code or third-party tracking SDK in the app. You can verify it on the App Store listing: under "App Privacy", Charty declares "Data Not Collected".

## What stays on your device

Charty stores the following locally, on your iPhone/iPad, using Apple's SwiftData framework:

- Charts, tasks, and schedules you create
- Your child's first name and (optionally) an avatar image you pick
- The rewards you define and the current points balance
- Session history (which routines were completed, when, points earned)
- Settings preferences (sound, haptics, animations, parent PIN hash, biometric preference)
- Custom task photos, if you choose to attach any from your Photos library

All of this lives on your device. None of it leaves your device unless **you** explicitly export it.

## Things you can do that involve your device leaving the app

The following features hand data to **iOS itself**, which then routes it under your control. Charty never sees or stores the result:

- **Print or share as PDF** — Charty generates a PDF locally and presents the iOS share sheet. You decide whether to AirPrint, save to Files, email, message, etc.
- **Export sessions as CSV** — Same pattern: file generated locally, share sheet hands it to whatever app you pick.
- **iCloud sync** (planned, off by default) — When enabled in a future version, your data will sync via CloudKit's **private database**, which is encrypted by Apple and tied to your own iCloud account. Charty's developer cannot read your iCloud private database. Sync is opt-in.

## Children's privacy

Charty is designed for children, primarily ages 4–10, including children with developmental disabilities such as autism spectrum disorder (ASD).

We comply with COPPA (US) and GDPR-K (EU) **by design**: we collect no data from anyone — children or adults — so there is nothing to consent to, nothing to process, nothing to delete.

The parent gate (4–6 digit PIN or Face ID / Touch ID) ensures only adults can change Settings, edit charts, or reset the points balance.

## Camera & Photos

If you tap "Pick a photo" for a task icon or for the picture-puzzle reward, iOS shows its standard photo picker. The photo you choose is **copied** into the app's local sandbox (downscaled and JPEG-compressed for the puzzle case). Photos never leave your device.

Charty does not request camera access. If you want to use a fresh photo, take it with the Photos app first and then pick it via the photo picker.

## Face ID / Touch ID

If you enable biometric unlock for the parent gate, authentication is handled entirely by Apple's local-only Face ID / Touch ID system. The biometric data never leaves your device's Secure Enclave, and Charty never sees it — we only receive a "success" or "fail" callback from iOS.

## Notifications

Charty schedules **local** notifications for daily routine reminders. These are managed by iOS and do not involve any server. You can disable them per-chart, or globally via iOS Settings → Notifications → Charty.

## Network access

Charty does **not** make any network requests. The app has no embedded URLs, no telemetry endpoints, no remote configuration, no ad SDKs, no analytics SDKs, no crash reporters. If you put the device in Airplane mode, Charty works identically.

## Changes to this policy

If this policy changes, the new version replaces this file in the public repository. Material changes will be noted at the top with a new effective date. Because no data is collected, there is no historical data to migrate or repurpose.

## Contact

📧 **Email:** ppeltriaux@gmail.com

Questions, concerns, or independent verification requests welcome.
