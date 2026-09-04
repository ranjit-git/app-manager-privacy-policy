# Privacy Policy

**Effective Date:** July 31, 2026  

## 1. Introduction

Welcome to **App Manager: Analyze & Backup** ("we," "our," or "us"). We are committed to protecting your privacy and ensuring that your personal information remains secure. This Privacy Policy explains how our application handles data on your device.

Our core philosophy is privacy-first. The application is designed to operate primarily on-device and does not require account creation to use its core features.

However, the app uses **Firebase** for crash reporting and basic interaction analytics to help us improve app stability and measure engagement.

## 2. Data Collection and Usage

**App Manager operates primarily locally on your device.**

We do **not** use external servers to harvest your personal data. Any sensitive data generated, analyzed, or displayed by the app (including app lists, screen time, storage metrics, and backups) remains strictly on your device unless you explicitly choose to export or share it.

### Crash and Diagnostic Information
The app uses **Firebase Crashlytics** to monitor crashes and technical issues. If the app crashes, limited technical information (crash logs, device model, app version) is transmitted to help us fix stability issues.

### Analytics and Interaction Tracking
We use **Firebase Analytics** to understand how users interact with our cross-promotion features (such as the "More Apps" page). We collect limited, anonymized event data (such as which promoted app was clicked) to measure engagement and improve our app ecosystem. This data does not personally identify you.

## 3. Required Permissions and Why We Need Them

To provide its core functionality, App Manager requires certain Android permissions. These permissions are used exclusively to provide features within the app and are never used to harvest data.

*   **`QUERY_ALL_PACKAGES` (Query All Packages):**
    *   *Purpose:* Required to list all user and system applications installed on your device so you can manage, back up, and analyze them.

*   **`PACKAGE_USAGE_STATS` (Usage Access):**
    *   *Purpose:* Required for the "Insights" dashboard to display screen time, network consumption, and storage usage metrics. This data is processed locally and never leaves your device.

*   **`REQUEST_DELETE_PACKAGES` (Delete Packages):**
    *   *Purpose:* Allows the app to prompt you to uninstall applications when you select the "Uninstall" or "Batch Uninstall" features.

*   **Note on Storage Access:** 
    *   *Purpose:* Unlike many app managers, this app is designed to maximize your privacy by **not** requesting broad storage permissions (`READ_EXTERNAL_STORAGE` or `MANAGE_EXTERNAL_STORAGE`). Instead, it uses modern Android Scoped Storage and the native Android Share Sheet, allowing you to save or share extracted APKs precisely where you want them without granting the app blanket access to your personal files.

## 4. Third-Party Services

The app uses **Firebase Crashlytics** and **Firebase Analytics**, provided by **Google LLC**.

- **Crashlytics** is used to monitor app crashes and improve reliability by processing technical information.
- **Analytics** is used to measure user engagement with features like the "More Apps" screen by logging anonymous interaction events using the Advertising ID.

More information about Firebase privacy and security is available here:  
[https://firebase.google.com/support/privacy](https://firebase.google.com/support/privacy)

We do **not** integrate third-party advertising networks that track your behavior across other apps and websites.

## 5. Data Sharing and Disclosure

We do **not** sell your personal data and do **not** share personal information for advertising or marketing purposes.

Crash-related technical and anonymous interaction data may be processed by Firebase as part of the reporting services used by the app.

The only way sensitive data leaves the app is if you manually choose to export and share it (for example, sharing an extracted APK or backup snapshot via the Android Share Sheet).

## 6. Children's Privacy (COPPA)

The app is not directed to children under the age required by applicable law for independent consent in their jurisdiction.

The app is not intended to knowingly collect personal information from children. If it is discovered that personal information from a child has been collected inadvertently, reasonable steps will be taken to delete it.

## 7. GDPR and CCPA Compliance

The app is designed with data minimization and privacy-by-design principles in mind. Most functionality operates on-device, and we limit stored information to what is needed for app features.

We do not collect, process, or store personal data off-device except for limited diagnostic and anonymous interaction data processed by Firebase as described above.

*   **Right to Erasure / Right to be Forgotten:** You have full control over your data. You can delete any backups or extracted APKs directly through your device's file manager. Uninstalling the app removes all associated local configurations.

## 8. Changes to This Privacy Policy

We may update this Privacy Policy from time to time if we introduce new features that require different device permissions or data handling. If any changes occur, we will update this document and the "Effective Date" at the top. We encourage you to review this policy periodically.

## 9. Contact Us

If you have any questions or concerns about this Privacy Policy or how App Manager handles your device permissions, please contact us at:

**Email:** [pahan.ranjit.0201@gmail.com](mailto:pahan.ranjit.0201@gmail.com)
