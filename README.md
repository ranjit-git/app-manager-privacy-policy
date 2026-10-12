# Privacy Policy

**Effective Date:** October 12, 2026  

## 1. Introduction

Welcome to **App Manager: Analyze & Backup** ("we," "our," or "us"). We are committed to protecting your privacy and ensuring that your personal information remains secure. This Privacy Policy explains how our application collects, uses, processes, and protects your information.

Our core philosophy is **privacy-first**:
* The application operates primarily **locally on your device**.
* We do **not** run private servers to harvest your personal data.
* No account creation, login, or registration is required to use any feature of the application.

To support the development and maintenance of the application, we integrate industry-standard Google services for **in-app advertising (Google AdMob)**, **in-app purchases (Google Play Billing)**, **crash reporting (Firebase Crashlytics)**, and **basic telemetry (Firebase Analytics)**.

---

## 2. On-Device Processing (Zero Harvest Philosophy)

The core features of App Manager—including installed application inspection, memory usage, screen time, network consumption tracking, APK extraction, and local backups—are executed **entirely on your local device**. 

We do **not** transmit, upload, or sell your list of installed applications, storage metrics, or backup files to external servers. Any extracted files remain exclusively in your private device storage unless you explicitly choose to share or export them using the native Android Share Sheet.

---

## 3. Data Collection and Third-Party Services

While the app's utility features run locally, we integrate trusted third-party SDKs provided by **Google LLC** to support analytics, crash diagnostics, monetization, and in-app billing.

### A. Advertising (Google AdMob)
We display banner, interstitial, and app-open advertisements provided by **Google AdMob**. To serve these ads, Google Mobile Ads SDK may collect and process:
* **Advertising ID (Google Play Advertising ID / `AD_ID`):** Used to deliver personalized or non-personalized advertisements, limit ad repetition, and combat click fraud.
* **Device Identifiers & Technical Specs:** Device model, screen orientation, operating system version, carrier, and general hardware performance.
* **Ad Interaction Metrics:** Ad impressions, clicks, and viewability telemetry.
* **Coarse Location Data:** General geographic location derived from your IP address (country or city level) to display relevant advertisements.

### B. In-App Purchases (Google Play Billing)
We offer an optional one-time purchase ("Remove Ads") that permanently removes all advertisements. 
* All financial transactions, billing processing, credit card details, and payment validations are handled **exclusively by Google Play**.
* We do **not** collect, store, or have access to your credit card, bank details, or financial accounts. 
* The app only receives an encrypted receipt token from Google Play to verify that your ad-free status is active.

### C. Crash Reporting (Firebase Crashlytics)
To help us diagnose and fix bugs, the app uses **Firebase Crashlytics**. If an unexpected error or crash occurs, technical data is collected:
* Stack traces and error logs.
* Device state at the time of the crash (e.g., RAM usage, device orientation, OS version).
* Crashlytics installation UUIDs.
* This information is strictly used for bug fixing and app stability, and is never sold or shared with advertisers.

### D. Analytics (Firebase Analytics)
We use **Firebase Analytics** to understand general user interactions (e.g., total sessions, screen visits, engagement with the "More Apps" screen). This data is aggregated and anonymized to help us optimize the app experience.

---

## 4. Required Android Permissions and Purpose

To deliver its core utility functions, App Manager requires certain Android permissions. These permissions are used strictly for local operations:

* **`QUERY_ALL_PACKAGES` (Query All Packages):**
  * *Purpose:* Required to scan, list, and categorize all user and system applications installed on your device so you can manage, back up, and analyze them. This data never leaves your device.
* **`PACKAGE_USAGE_STATS` (Usage Access):**
  * *Purpose:* Required for the "Insights" dashboard to display screen time, network consumption, and storage usage metrics. All statistics are calculated entirely on-device.
* **`REQUEST_DELETE_PACKAGES` (Delete Packages):**
  * *Purpose:* Allows the app to request the system package installer to prompt you for application uninstallation when you choose to uninstall an app.
* **`INTERNET` & `ACCESS_NETWORK_STATE`:**
  * *Purpose:* Required to check internet connectivity, load advertisements, verify In-App Purchases via Google Play, and send crash reports to Firebase.
* **`com.google.android.gms.permission.AD_ID` (Advertising ID):**
  * *Purpose:* Required on Android 13+ devices to allow Google AdMob to access the Advertising ID for ad serving and fraud prevention.
* **`com.android.vending.BILLING` (Google Play Billing):**
  * *Purpose:* Required to connect with the Google Play Store to process the "Remove Ads" in-app purchase and restore past purchases.
* **Note on Storage Access:** 
  * The app respects your privacy by **not** requesting broad legacy storage permissions (`READ_EXTERNAL_STORAGE` or `MANAGE_EXTERNAL_STORAGE`). Extracted APKs and backups are managed safely via modern Android Scoped Storage and the native Android Share Sheet.

---

## 5. In-App Purchases & The "Zero-Ad Guarantee"

If you purchase the **"Remove Ads"** upgrade:
1. All banner, interstitial, and app-open advertisements are permanently disabled.
2. The Google Mobile Ads SDK is prevented from making network requests or loading ad units.
3. No further advertising data or ad-interaction telemetry will be collected or shared by the app.

You can restore your purchase at any time on any device linked to your Google Play account by tapping **"Restore Purchases"** in the Settings or App Drawer.

---

## 6. European Privacy Rights (GDPR) & Consent Management

For users located in the **European Economic Area (EEA), the United Kingdom (UK), and Switzerland**:

We comply with the **General Data Protection Regulation (GDPR)** and Google's EU User Consent Policy using the official **Google User Messaging Platform (UMP)** SDK:
* **Consent Dialog:** On your first launch, you are presented with a consent form powered by the IAB Europe Transparency and Consent Framework (TCF v2.2), allowing you to consent to or manage choices regarding personalized ads, non-personalized ads, and data storage.
* **Revoking or Modifying Consent:** You have the legal right to change or withdraw your consent at any time. You can do this directly inside the app by going to **Settings > Privacy & Ad Settings (Manage data consent)**.

---

## 7. California Privacy Rights (CCPA / CPRA)

Under the **California Consumer Privacy Act (CCPA)** and the **California Privacy Rights Act (CPRA)**:
* We do **not** sell your personal information for monetary value.
* We do **not** collect sensitive personal information such as government IDs, precise geolocation, racial or ethnic origin, or biometric data.
* You have the right to know what information is collected, request its deletion, and not receive discriminatory treatment for exercising your privacy rights.

---

## 8. Children's Privacy (COPPA)

App Manager is a general utility tool and is **not directed to children under the age of 13** (or the age of digital consent in your jurisdiction). We do not knowingly collect personal information from children. If you are a parent or guardian and believe that your child has provided personal information to third-party SDKs through our app, please contact us, and we will take immediate steps to remove such data.

---

## 9. Data Security and Retention

* **Data in Transit:** All communications with Google services (AdMob, Firebase, Google Play Billing) are encrypted using industry-standard **HTTPS / TLS** encryption.
* **Data Retention:** Since we do not host external databases, we retain no personal data on our own servers. Any locally saved preferences (such as your chosen theme or favorite apps) can be erased at any time by clearing the app's cache/storage in your device settings or by uninstalling the application.

---

## 10. Third-Party Links & Policies

Our app may contain links to external websites (such as our developer store page or third-party app listings in "More Apps"). We are not responsible for the content or privacy practices of external websites. We encourage you to review their respective privacy policies:
* [Google Privacy & Terms](https://policies.google.com/privacy)
* [Google AdMob Policies](https://support.google.com/admob/answer/6128543)
* [Firebase Privacy Information](https://firebase.google.com/support/privacy)

---

## 11. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in legal requirements, device permissions, or app functionality. When changes are made, we will update the "Effective Date" at the top of this page. We encourage you to review this policy periodically.

---

## 12. Contact Us

If you have any questions, feedback, or concerns regarding this Privacy Policy or how your data is handled, please contact us at:

* **Developer Email:** [pahan.ranjit.0201@gmail.com](mailto:pahan.ranjit.0201@gmail.com)
