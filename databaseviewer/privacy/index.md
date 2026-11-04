---
redirect_from:
  - /accessviewer/privacy/
---
# AccessViewer Privacy Policy

**Product:** Database Viewer: MDB & ACCDB (AccessViewer)  
**Effective Date:** August 19, 2026  
**Last Updated:** November 4, 2026

This Privacy Policy explains how Database Viewer (AccessViewer, the “App”) handles information in the iOS and Android versions published by W4N9WE1.

## 1. Local database processing

AccessViewer is designed to process Microsoft Access database files locally on your device. Files you select, including `.mdb` and `.accdb` files, are copied to the App’s private storage when needed for parsing and browsing. Database contents, health reports, local query results, and exports remain on your device unless you explicitly share or export them.

The App does not require an account, and it does not upload your original database file as part of normal browsing, diagnostics, SQL, or export workflows.

## 2. Current feature status

The current Android release does not expose an AI Query entry point. The implementation is retained for possible future evaluation. If the feature is restored, this policy will be updated before it becomes available.

## 3. Advertising, analytics, and consent

The free version may display banner advertising through Google AdMob and may show an occasional interstitial ad. Interstitial ads are rate-limited and are not required to open or browse a database. Google may process device, advertising, diagnostic, and approximate location information as described in [Google’s Privacy Policy](https://policies.google.com/privacy). Where required, the App uses Google’s User Messaging Platform (UMP) to request consent and provide advertising privacy options, and Pro users do not see ads.

The App also uses PostHog to record limited, pseudonymous usage analytics: app opens, screen views, feature-usage events (such as opening a database file or reaching a preview limit), paywall interactions, and purchase-result events. Events are linked to a random, device-scoped identifier that is not connected to your name, email, or database contents, and no file names, table names, SQL text, or database contents are ever included in analytics events. Where the App presents a paywall or records a purchase, RevenueCat may share subscription status with PostHog under the same pseudonymous identifier so that purchase and usage analytics stay consistent.

PostHog also records optional, masked session replays to diagnose usability problems and crashes. Replays render screens as masked wireframes: text and images are replaced with placeholders before they leave the device, so replays do not contain readable screen content. Data handled by PostHog is stored on PostHog’s cloud in the United States. See [PostHog’s Privacy Policy](https://posthog.com/privacy).

Where required by applicable law (for example, in the EEA and the UK), the App asks for your consent before enabling personalized advertising, analytics, and session replay, and you can decline without losing any App functionality. You may also opt out later through the App’s privacy-options UI or by contacting us at the address below; previously collected pseudonymous analytics remain subject to PostHog’s retention practices.

## 4. AI query requests (future feature reference)

When you explicitly use the AI Query feature, the App sends a request to the App’s relay service at `relay.access-db-viewer.com`. The request may contain:

- The natural-language question you entered.
- Sanitized database schema information, such as table names, column names, and data types.

The App is designed not to send the original MDB/ACCDB file or a full database dump in an AI request. The relay and its AI providers may process the request to return a SQL query and explanation. Do not include confidential information in an AI question or database field name if you do not want it sent to the relay.

## 5. Purchases and subscriptions

AccessViewer Pro is provided through Apple In-App Purchases and Google Play Billing, with entitlement managed by RevenueCat. When you view a paywall, purchase, restore, or manage a purchase, Apple, Google Play, and RevenueCat may process purchase records, transaction information, subscription status, and a pseudonymous App User ID to provide entitlement and restore functionality.

The App uses the `AccessViewer Pro` entitlement to determine access to Pro features. See [RevenueCat’s Privacy Policy](https://www.revenuecat.com/privacy/), [Apple’s privacy information](https://www.apple.com/privacy/), and [Google Play’s privacy information](https://policies.google.com/privacy) for the providers’ handling of this information.

The App does not receive or store your payment card number or bank details.

## 6. Diagnostics, crash reports, and usage analytics

The App may process technical information required to operate the App, such as device and operating-system details, app version, file format, file size, and error details. These details are used to provide file diagnostics and explain failures.

The App uses Google Firebase Crashlytics to collect crash and error reports. Crash reports may include device model and manufacturer, operating-system and app versions, stack traces, and related technical identifiers, and are used to diagnose and fix crashes.

The App uses PostHog for product analytics as described in Section 3 (usage events, screen views, masked session replay, and purchase-result events, tied to a random device-scoped identifier). Google processes Crashlytics information as described in [Google’s Privacy Policy](https://policies.google.com/privacy), and PostHog processes analytics information as described in [PostHog’s Privacy Policy](https://posthog.com/privacy).

The current Android workflow does not require a user account.

## 7. Sharing and retention

We do not sell your personal information. Local files, reports, cached copies, and exports remain on your device until you delete them, clear the App’s data, or uninstall the App. Information handled by Google, PostHog, RevenueCat, or the AI relay is subject to those providers’ retention practices and policies.

You control any file or report that you explicitly export or share with another app or service.

## 8. Children’s privacy

AccessViewer is not directed to children under 13, and we do not knowingly collect personal information from children under 13 through the App.

## 9. Security

The App uses Android private storage and platform file-access permissions for local processing. No method of storage or transmission can guarantee absolute security. Do not open files you are not authorized to access, and avoid sending confidential content in AI questions.

## 10. Changes to this policy

We may update this Privacy Policy when the App or its supporting services change. The latest version will be published on this page with an updated date.

## 11. Contact

For privacy questions or requests, contact [w4n9we1@gmail.com](mailto:w4n9we1@gmail.com?subject=AccessViewer%20Privacy%20Question).
