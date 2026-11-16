# SoloSide Privacy Policy

**Last Updated:** November 16, 2026

SoloSide is an iPhone app published by W4N9WE1. It records custody handoffs, parenting time, expenses and attachments on your device, and exports them as PDF, xlsx and calendar files. This policy describes exactly what is processed, where it stays, and what leaves your phone.

**Short version:** your custody record is not uploaded to us. There is no SoloSide account and no SoloSide server holding your entries. We cannot read your notes, photos or your children's information.

## 1. Data stored on your iPhone

To provide its features, SoloSide stores the following locally in the app's own storage:

- Handoff entries: status, timestamps, optional place and distance, notes.
- Attachments you add: photos, scanned receipts, PDFs.
- Expenses: amount, currency, category, optional receipt reference.
- Custody factors you tag on entries.
- Schedule templates, overrides and imported calendar data.
- Every entry's SHA-256 fingerprint and the chain values used for tamper detection.
- Amendment history (original value, corrected value, timestamps) and audit entries for deletions and bulk changes.
- Local automatic snapshots retained for 30 days so a corrupted database can be rolled back.
- Text produced by on-device transcription of a chat screen recording you choose to import.
- App preferences, and cached store product information.

Deleting an entry removes it from the working set; audit entries, and any copy inside a local snapshot, may remain until the snapshot expires. "Delete all data" in Settings clears the record and its snapshots after a confirmation.

## 2. Data that leaves your device

SoloSide does not upload your custody record. It has no backend service. The only outbound processing is:

- **Purchases (RevenueCat).** Apple processes payment. SoloSide uses RevenueCat to load products, validate entitlement and support Restore Purchases. RevenueCat receives an anonymous app user ID, product and transaction information, entitlement status, and technical app/device information needed for that service. Your entries, photos, notes, expenses and children's names are never sent to RevenueCat. See [RevenueCat Privacy Policy](https://www.revenuecat.com/privacy/).
- **Analytics and crash reports (Firebase).** SoloSide uses Firebase Analytics and Crashlytics to understand which features are used and to receive crash diagnostics. These events contain app-level actions (for example "export completed"), device model, iOS version, app version and a pseudonymous installation identifier. They do not contain your notes, photos, places, expenses, children's names or any content of your record.
- **iCloud sync, only if you enable it.** Your record is written to your own private iCloud container tied to your Apple ID. It is not routed through SoloSide.
- **What you share.** When you export or share a file, it goes where you send it: Files, Mail, Messages, AirDrop, a lawyer. That destination's privacy policy governs it. The attorney export package is built on your device and handed to whoever you send it to.

SoloSide does not include third-party advertising SDKs and does not sell data.

## 3. Verification pages

A SoloSide export includes a hash list. Verification runs entirely in the browser: the page computes SHA-256 of the file you select and compares it with the value printed in the export. No file, hash or identifier is transmitted to us, and nothing is logged on a server, because there is no server. In this version SoloSide does not request third-party timestamps; if that changes, it will be opt-in and only a fingerprint — never your content — would leave the device, and this policy will be updated first.

## 4. Permissions

- **Photos / Camera.** Used only when you attach a photo or receipt. SoloSide does not scan your library in the background.
- **Notifications.** Local reminders for upcoming handoffs. Scheduled on the device; no push server is involved.
- **Face ID / Touch ID.** Optional app lock via Apple's LocalAuthentication. Biometric data never leaves the Secure Enclave and is not available to SoloSide.
- **iCloud.** Only for sync, and only if you turn it on.
- **Microphone / Speech recognition.** Used only when you import a screen recording for transcription. Processing happens on the device with Apple's on-device speech recognition; the recording and the resulting text are not uploaded. If on-device recognition is unavailable for your language, SoloSide shows an error instead of uploading the media.

## 5. Children's information

Your record may describe your children: names, schools, handoff times, photos. That information is stored on your device (and in your own iCloud if you enable sync). We do not collect it, cannot read it, and do not receive it. You are responsible for what you record and for who can physically access your phone.

## 6. Retention and deletion

Local data stays until you delete it, delete the app, or clear it in Settings. Snapshots expire automatically after 30 days. Purchases and entitlement records are retained by Apple and RevenueCat under their policies, because they are financial records. Analytics data is retained by Firebase under Google's retention settings for the project.

## 7. Security

Records are held in the app's private container protected by iOS. Optional Face ID lock adds device-level access control. Fingerprints and the amendment/audit trail make silent modification detectable. No system is perfect: if your device is unlocked and shared, someone can read the app. Use the lock and your passcode.

## 8. Your choices

- Disable analytics: iOS Settings → Privacy & Security → Analytics, or contact us and we will document the opt-out path for the current version.
- Disable iCloud sync, notifications or Face ID lock at any time in the app or in iOS Settings.
- Export your data at any time (PDF / xlsx / ICS). Pro enables full-history export; the free tier includes the current month.

## 9. Contact

Questions about this policy: [w4n9we1@gmail.com](mailto:w4n9we1@gmail.com?subject=SoloSide%20Privacy).

We may update this policy as the app changes; the "Last Updated" date above shows the current version, and material changes will be described in the app's release notes.

- [Support](../support/) · [Terms of Use](../terms/)
