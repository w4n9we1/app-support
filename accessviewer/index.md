# AccessViewer Privacy Policy

**Product:** AccessViewer (Access Database Viewer)  
**Effective Date:** August 19, 2026  
**Last Updated:** August 24, 2026

This Privacy Policy explains how AccessViewer (the “App”) handles information in the Android version published by W4N9WE1.

## 1. Local database processing

AccessViewer is designed to process Microsoft Access database files locally on your device. Files you select, including `.mdb` and `.accdb` files, are copied to the App’s private storage when needed for parsing and browsing. Database contents, health reports, local query results, and exports remain on your device unless you explicitly share or export them.

The App does not require an account, and it does not upload your original database file as part of normal browsing, diagnostics, SQL, or export workflows.

## 2. Current feature status

The current Android release does not expose an AI Query entry point. The implementation is retained for possible future evaluation. If the feature is restored, this policy will be updated before it becomes available.

## 3. Advertising and consent

The free version may display banner advertising through Google AdMob and may show an occasional interstitial ad when you replace an already-open database file. Interstitial ads are rate-limited and are not required to open or browse a database. Google may process device, advertising, diagnostic, and approximate location information as described in [Google’s Privacy Policy](https://policies.google.com/privacy).

Where required, the App uses Google’s User Messaging Platform (UMP) to request consent and provide privacy options. You can change available advertising privacy choices through the consent or privacy options UI. Pro users do not see banner or interstitial ads, and the App does not actively load new ad requests for Pro users.

## 4. AI query requests (future feature reference)

When you explicitly use the AI Query feature, the App sends a request to the App’s relay service at `relay.access-db-viewer.com`. The request may contain:

- The natural-language question you entered.
- Sanitized database schema information, such as table names, column names, and data types.

The App is designed not to send the original MDB/ACCDB file or a full database dump in an AI request. The relay and its AI providers may process the request to return a SQL query and explanation. Do not include confidential information in an AI question or database field name if you do not want it sent to the relay.

## 5. Purchases and subscriptions

AccessViewer Pro is provided through Google Play Billing and RevenueCat. When you view a paywall, purchase, restore, or manage a purchase, Google Play and RevenueCat may process purchase records, transaction information, subscription status, and a pseudonymous App User ID to provide entitlement and restore functionality.

The App uses the `AccessViewer Pro` entitlement to determine access to Pro features. See [RevenueCat’s Privacy Policy](https://www.revenuecat.com/privacy/) and [Google Play’s privacy information](https://policies.google.com/privacy) for the providers’ handling of this information.

The App does not receive or store your payment card number or bank details.

## 6. Diagnostics and technical information

The App may process technical information required to operate the App, such as device and operating-system details, app version, file format, file size, and error details. These details are used to provide file diagnostics and explain failures. The current Android workflow does not require a user account.

## 7. Sharing and retention

We do not sell your personal information. Local files, reports, cached copies, and exports remain on your device until you delete them, clear the App’s data, or uninstall the App. Information handled by Google, RevenueCat, or the AI relay is subject to those providers’ retention practices and policies.

You control any file or report that you explicitly export or share with another app or service.

## 8. Children’s privacy

AccessViewer is not directed to children under 13, and we do not knowingly collect personal information from children under 13 through the App.

## 9. Security

The App uses Android private storage and platform file-access permissions for local processing. No method of storage or transmission can guarantee absolute security. Do not open files you are not authorized to access, and avoid sending confidential content in AI questions.

## 10. Changes to this policy

We may update this Privacy Policy when the App or its supporting services change. The latest version will be published on this page with an updated date.

## 11. Contact

For privacy questions or requests, contact [w4n9we1@gmail.com](mailto:w4n9we1@gmail.com?subject=AccessViewer%20Privacy%20Question).
