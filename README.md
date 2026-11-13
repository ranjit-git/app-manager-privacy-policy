# Privacy Policy

**Effective Date:** October 12, 2026  
**Last Updated:** November 14, 2026  

## 1. Introduction

Welcome to **App Manager: Analyze & Backup** ("we," "our," or "us"), developed by **Ranjit Pahan**. We are deeply committed to protecting your privacy and ensuring that your personal information remains secure. This Privacy Policy explains how our application operates, what information is processed, and how third-party services are utilized.

Our core philosophy is **privacy-first and zero-harvest**:
* The application operates primarily **locally on your device**.
* We do **not** run private servers to harvest, collect, or monetize your personal data.
* No account creation, login, or registration is required to use any feature of the application.

To support the ongoing maintenance and quality of the application, we integrate industry-standard Google developer services for **in-app advertising (Google AdMob)**, **in-app purchases (Google Play Billing)**, **crash reporting (Firebase Crashlytics)**, **telemetry (Firebase Analytics)**, and **dynamic configuration (Firebase Remote Config)**.

---

## 2. On-Device Processing (Zero Harvest Philosophy)

The core utility features of App Manager—including installed application inspection, component analysis (Activities, Services, Receivers, Providers), memory metrics, screen time analysis, network consumption tracking, APK extraction, and local backup snapshots—are executed **entirely on your local device**.

We do **not** transmit, upload, or sell your list of installed applications, package metadata, storage metrics, or backup files to external servers. Any extracted files remain exclusively in your private device storage or public Downloads folder unless you explicitly choose to share or export them using the native Android Share Sheet.

---

## 3. Data Collection and Third-Party Services

While the app's utility features run locally, we integrate trusted third-party SDKs provided by **Google LLC** to support analytics, crash diagnostics, monetization, in-app billing, and remote configuration.

### A. Advertising (Google AdMob)
We display banner, interstitial, and app-open advertisements provided by **Google AdMob**. To serve these ads, the Google Mobile Ads SDK may collect and process:
* **Advertising ID (Google Play Advertising ID / `AD_ID`):** Used to deliver personalized or non-personalized advertisements, limit ad repetition (frequency capping), and combat invalid traffic or click fraud.
* **Device Identifiers & Technical Specs:** Device model, screen orientation, operating system version, carrier, and general hardware performance.
* **Ad Interaction Metrics:** Ad impressions, clicks, viewability telemetry, and aggregated ad revenue metrics logged via Firebase Analytics (`onPaidEvent`) to evaluate ad performance.
* **Coarse Location Data:** General geographic location derived from your IP address (country or city level) to display relevant advertisements.

### B. In-App Purchases (Google Play Billing)
We offer an optional one-time purchase ("Remove Ads") that permanently removes all advertisements from the application.
* All financial transactions, billing processing, credit card details, and payment validations are handled **exclusively by Google Play**.
* We do **not** collect, store, or have access to your credit card, bank details, or financial accounts. 
* The app only receives an encrypted receipt token from Google Play to verify that your ad-free status is active.

### C. Crash Reporting (Firebase Crashlytics)
To help us diagnose and fix bugs and performance issues, the app uses **Firebase Crashlytics**. If an unexpected error or crash occurs, technical data is collected:
* Stack traces and error logs.
* Device state at the time of the crash (e.g., free RAM, storage, device orientation, OS version).
* Crashlytics installation UUIDs.
* This information is strictly used for bug fixing and app stability, and is never sold or shared with third-party advertisers.

### D. Analytics & Remote Configuration (Firebase)
* **Firebase Analytics:** Used to understand general user interactions (e.g., total sessions, screen views, feature engagement). All analytics data is aggregated and anonymized.
* **Firebase Remote Config:** Fetches dynamic application configurations (such as ad cooldown intervals, feature toggles, app update notifications, and updated privacy policy links). No personally identifiable information is sent to or stored in Remote Config.

### E. Google Play In-App Review
The app may periodically invoke the official Google Play In-App Review API to allow you to rate and review the app. This interaction takes place directly between your device and the Google Play Store; we do not collect or store your review data.

---

## 4. Required Android Permissions and Purpose

To deliver its core management functions, App Manager requires specific Android permissions. These permissions are used strictly for local operations:

* **`android.permission.QUERY_ALL_PACKAGES` (Query All Packages):**
  * *Purpose:* Required to scan, list, and categorize all user and system applications installed on your device so you can manage, back up, and analyze them. This data is processed purely in memory and never leaves your device.
* **`android.permission.PACKAGE_USAGE_STATS` (Usage Access):**
  * *Purpose:* Required for the "Insights" dashboard to display:
    1. Per-app storage breakdowns (App, Data, and Cache size via `StorageStatsManager`).
    2. Screen time and foreground app usage (via `UsageStatsManager`).
    3. Network data consumption (Wi-Fi and mobile data TX/RX bytes via `NetworkStatsManager`).
  * *Control:* This is a special system access permission. It is never enabled automatically; users are directed to system settings via `Settings.ACTION_USAGE_ACCESS_SETTINGS` and can grant or revoke it at any time.
* **`android.permission.REQUEST_DELETE_PACKAGES` (Delete Packages):**
  * *Purpose:* Allows the app to prompt the native Android system package installer when you choose to uninstall an application. Every uninstallation requires explicit user confirmation.
* **`android.permission.INTERNET` & `android.permission.ACCESS_NETWORK_STATE`:**
  * *Purpose:* Required to check internet connectivity, load advertisements, verify In-App Purchases via Google Play, fetch Remote Config settings, and send crash diagnostics.
* **`com.google.android.gms.permission.AD_ID` (Advertising ID):**
  * *Purpose:* Required on Android 13+ devices to allow Google AdMob to access the Advertising ID for ad serving, frequency capping, and fraud prevention.
* **`com.android.vending.BILLING` (Google Play Billing):**
  * *Purpose:* Required to connect with the Google Play Store to process the "Remove Ads" in-app purchase and restore past purchases.
* **Note on Storage Access:** 
  * The app respects your privacy by **not** requesting broad legacy storage permissions (`READ_EXTERNAL_STORAGE` or `MANAGE_EXTERNAL_STORAGE`).
  * Extracted APKs are saved directly to your public Downloads directory (`/Download/AppManagerBackups`) or staged in the app's private cache for sharing via Android's secure `FileProvider`.
  * Backup metadata snapshots (`.json` files) are exported and imported using the standard Android Storage Access Framework via the system file picker.

---

## 5. In-App Purchases & The "Zero-Ad Guarantee"

If you purchase the **"Remove Ads"** upgrade:
1. All banner, interstitial, and app-open advertisements are permanently disabled.
2. The Google Mobile Ads SDK is silenced and prevented from making ad fetch requests.
3. No further advertising data or ad-interaction telemetry will be collected or processed by the app.

You can restore your purchase at any time on any device linked to your Google Play account by tapping **"Restore Purchases"** in the Settings screen or App Drawer.

---

## 6. European Privacy Rights (GDPR / UK GDPR) & Consent Management

For users located in the **European Economic Area (EEA), the United Kingdom (UK), and Switzerland**:

We comply with the **General Data Protection Regulation (GDPR)** and Google's EU User Consent Policy using the official **Google User Messaging Platform (UMP)** SDK:
* **Consent Dialog:** On your first launch, you are presented with a consent form powered by the IAB Europe Transparency and Consent Framework (TCF v2.2), allowing you to consent to or manage choices regarding personalized ads, non-personalized ads, and data storage.
* **Revoking or Modifying Consent:** You have the legal right to change or withdraw your consent at any time. You can do this directly inside the app by navigating to **Settings > Privacy & Ad Settings (Manage data consent)**.

---

## 7. California Privacy Rights (CCPA / CPRA)

Under the **California Consumer Privacy Act (CCPA)** and the **California Privacy Rights Act (CPRA)**:
* We do **not** sell your personal information for monetary or other valuable consideration.
* We do **not** share your personal information for cross-context behavioral advertising without your consent.
* We do **not** collect sensitive personal information such as government IDs, precise geolocation, racial or ethnic origin, or biometric data.
* You have the right to know what information is collected, request its deletion, and not receive discriminatory treatment for exercising your privacy rights.

---

## 8. Children's Privacy (COPPA)

App Manager is a technical utility tool and is **not directed to children under the age of 13** (or the age of digital consent in your jurisdiction). We do not knowingly collect personal information from children. If you believe that a child has provided personal information to third-party SDKs through our app, please contact us immediately, and we will take steps to ensure such data is removed.

---

## 9. Data Security and Local Data Retention

* **Data in Transit:** All communications with Google services (AdMob, Firebase, Google Play Billing) are encrypted using industry-standard **HTTPS / TLS** protocols.
* **Zero Remote Server Retention:** Because we do not operate private servers or external databases, we retain no personal data externally.
* **Local Preferences:** Locally saved preferences (such as your chosen theme mode, favorite apps list, language selection, backup snapshots, and ad-free entitlement) are stored strictly within the app's private sandbox (`SharedPreferences`). You can erase this data at any time by clearing the app's storage in your device settings or by uninstalling the application.

---

## 10. Third-Party Links & Policies

Our app may contain links to external websites (such as our developer store page or third-party apps listed in "More Apps"). We are not responsible for the content or privacy practices of external websites. We encourage you to review their respective privacy policies:
* [Google Privacy & Terms](https://policies.google.com/privacy)
* [Google AdMob Policies](https://support.google.com/admob/answer/6128543)
* [Firebase Privacy Information](https://firebase.google.com/support/privacy)
* [Google Play In-App Review Policy](https://developer.android.com/guide/playcore/in-app-review)

---

## 11. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in legal requirements, device permissions, or app functionality. When changes are made, we will update the "Effective Date" and "Last Updated" timestamp at the top of this document. We encourage you to review this policy periodically.

---

## 12. Contact Us

If you have any questions, feedback, or concerns regarding this Privacy Policy or how your data is handled, please contact us at:

* **Developer:** Ranjit Pahan  
* **Developer Email:** [pahan.ranjit.0201@gmail.com](mailto:pahan.ranjit.0201@gmail.com)  
* **Privacy Policy URL:** [https://ranjit-git.github.io/app-manager-privacy-policy/](https://ranjit-git.github.io/app-manager-privacy-policy/)
