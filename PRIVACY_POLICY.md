# Privacy Policy

**Aksha — Personal Routine Tracker & Habit Management App**

**Effective Date:** 8 March 2026
**Last Updated:** 8 March 2026
**App Package Name:** aashu.aksha
**Version:** 1.6.2

---

## 1. Introduction

Welcome to Aksha ("we", "our", "us", or the "App"). Aksha is a personal routine tracker and habit management application designed to help users track their daily routines honestly and build better habits. We are committed to protecting your privacy and handling your data transparently, responsibly, and securely.

This Privacy Policy explains what information we collect, how we use it, how we store it, and what rights you have regarding your data. By installing and using Aksha, you agree to the terms described in this Privacy Policy.

---

## 2. Developer Information

- **Developer Name:** Aakash
- **Contact Email:** bamniyaaakash958@gmail.com
- **Country:** India

---

## 3. Information We Collect

### 3.1 Information You Provide Directly

| Data Type | Description | Purpose |
|-----------|-------------|---------|
| **Name** | Your display name (entered manually or obtained from Google account) | Personalisation of the app experience |
| **Email Address** | Google account email (only if Google Sign-In is used) | Account identification and Google Drive backup |
| **Profile Photo** | Google profile picture URL or a photo you pick from your gallery/camera | Profile display within the app |
| **Routine Data** | Routine names, categories, scheduled times, repeat days, and duration | Core app functionality — tracking routines |
| **Daily Activity Instances** | Status (done, partial, skipped, missed, pending), actual time spent, and personal notes | Daily tracking and insights |
| **Tags** | Custom labels (name, colour, emoji) you assign to routine instances | Organisation and filtering of routines |
| **Reflections** | Daily mood ratings (1–5 scale) and optional personal notes | Self-reflection and mood tracking |
| **Category Data** | Custom category names, colours, and icons you create | Organising routines into groups |

### 3.2 Information Collected Automatically

| Data Type | Description | Purpose |
|-----------|-------------|---------|
| **Gamification Stats** | XP points, level, streaks, and achievement badges | Motivational features within the app |
| **App Usage Metadata** | Schema version, onboarding completion status, theme preference | App functionality and settings persistence |
| **Crash Reports** | Stack traces, device model, OS version, and error logs (via Firebase Crashlytics) | Identifying and fixing bugs to improve app stability |

### 3.3 Information We Do NOT Collect

- ❌ **Location data** — We do not access or track your geographical location.
- ❌ **Contacts or phone book** — We do not access your contacts.
- ❌ **Call logs or SMS** — We do not access calls or messages.
- ❌ **Browsing history** — We do not track web activity.
- ❌ **Financial or payment information** — The app is free with no in-app purchases.
- ❌ **Unique device identifiers for advertising** — We do not use advertising SDKs.
- ❌ **Microphone or audio** — We do not record audio.

---

## 4. How We Use Your Information

We use the collected information **solely** for the following purposes:

1. **Core App Functionality** — To create, manage, and track your daily routines, categories, tags, reflections, and achievements.
2. **Personalisation** — To display your profile (name, photo) and apply your preferred theme.
3. **Data Backup & Restore** — To back up your data to your personal Google Drive account (only when you explicitly initiate a backup) and to restore it when needed.
4. **Insights & Analytics** — To generate personal performance charts, completion rates, streaks, and summary reports visible only to you within the app.
5. **Notifications** — To send locally scheduled reminders for your routines. These are **on-device notifications** and are **not** push notifications from a server.
6. **Home Screen Widget** — To display daily routine information on your Android home screen.
7. **Crash Reporting** — To collect anonymous crash data through Firebase Crashlytics to identify, diagnose, and fix technical issues.
8. **Data Export** — To allow you to export your routine data as a CSV file for your personal records.

---

## 5. Data Storage & Security

### 5.1 Local Storage (On-Device)

The majority of your data is stored **locally on your device** using the following mechanisms:

- **SQLite Database** (`aksha.db`) — Stores routines, daily instances, categories, tags, reflections, achievements, and user stats. This database is stored in your device's private application directory and is **not accessible** to other apps.
- **SharedPreferences** — Stores lightweight settings like user profile data (name, email, photo path), theme preference, onboarding status, and last backup time. This is stored in the app's private sandbox.
- **Local File System** — Profile photos (picked from gallery or camera) are saved in the app's private documents directory.

### 5.2 Cloud Storage (Optional — Google Drive)

- If you choose to use the **Google Drive Backup** feature, your routine and app data is encrypted and uploaded to your **personal Google Drive** account in the application-specific data folder (`appDataFolder`).
- This data is **only accessible by you** and by the Aksha app. No other apps or users can view this data.
- Backups are created **only when you manually initiate** them from the Settings screen. There is no automatic background upload of your data.

### 5.3 Firebase Services

- **Firebase Authentication** — Used solely to manage Google Sign-In. We store your Firebase UID, display name, and email only for authentication purposes.
- **Firebase Crashlytics** — Collects anonymous crash reports including stack traces, device type, OS version, and app version. **No personally identifiable routine data** is included in crash reports.

### 5.4 Security Measures

- All data stored on your device is in the app's **private sandboxed directory**, inaccessible to other applications.
- Google Drive communication uses **HTTPS encryption** for data in transit.
- Firebase services use **Google's enterprise-grade security infrastructure**.
- The app requests only the **minimum permissions** required for its functionality.

---

## 6. Permissions

The app requests the following Android permissions:

| Permission | Purpose | Required? |
|------------|---------|-----------|
| `INTERNET` | For Google Sign-In, Google Drive backup, and Firebase Crashlytics | Yes (for online features) |
| `ACCESS_NETWORK_STATE` | To check network availability before backup operations | Yes (for online features) |
| `POST_NOTIFICATIONS` | To send local routine reminders | Yes (for notifications) |
| `RECEIVE_BOOT_COMPLETED` | To re-schedule notifications after device restart | Yes (for notifications) |
| `VIBRATE` | To vibrate the device for notification alerts | Optional |
| `SCHEDULE_EXACT_ALARM` | To schedule precise routine reminders at exact times | Yes (for notifications) |
| `USE_FULL_SCREEN_INTENT` | To display timer/alarm notifications in full-screen mode | Yes (for timer feature) |
| `FOREGROUND_SERVICE` | To run the activity timer in the background | Yes (for timer feature) |
| `Camera` (runtime) | To take a profile photo using your camera | Optional |
| `Storage/Photos` (runtime) | To pick a profile photo from your gallery | Optional |

> **Note:** The `Camera` and `Storage/Photos` permissions are requested **at runtime** only when you choose to set a profile photo. You can deny these permissions and still use the app fully by choosing an emoji avatar instead.

---

## 7. Third-Party Services

Aksha integrates the following third-party services. Each has its own privacy policy:

| Service | Provider | Purpose | Privacy Policy |
|---------|----------|---------|----------------|
| **Firebase Authentication** | Google LLC | Google Sign-In for account management | [Firebase Privacy Policy](https://firebase.google.com/support/privacy) |
| **Firebase Crashlytics** | Google LLC | Anonymous crash reporting | [Firebase Privacy Policy](https://firebase.google.com/support/privacy) |
| **Google Sign-In** | Google LLC | Authentication via Google account | [Google Privacy Policy](https://policies.google.com/privacy) |
| **Google Drive API** | Google LLC | Optional data backup/restore to user's own Drive | [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy) |

### Google API Services Disclosure

Aksha's use and transfer of information received from Google APIs to any other app adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements. Specifically:

- We only request the `drive.file` scope, which limits access to files created by Aksha. We **cannot** access your other Google Drive files.
- Your Google Drive data is used **solely** for backup and restore functionality.
- We do **not** transfer, sell, or share your Google account data with any third parties.

---

## 8. Data Sharing & Disclosure

### We Do NOT:

- ❌ **Sell** your personal data to anyone.
- ❌ **Share** your data with advertisers or marketing companies.
- ❌ **Transfer** your data to third parties for their own purposes.
- ❌ **Use** your data for profiling, targeted advertising, or behavioural tracking.
- ❌ **Display** advertisements of any kind within the app.

### Limited Disclosure:

We may disclose information only in the following exceptional circumstances:

- **Legal Compliance** — If required by law, court order, or governmental authority.
- **Crash Data** — Anonymous, non-identifiable crash reports are sent to Firebase Crashlytics (Google) to help us improve app stability.

---

## 9. Data Retention

| Data Type | Retention Period | Deletion Method |
|-----------|-----------------|-----------------|
| **On-device data** (routines, instances, reflections, etc.) | Retained until you delete it or uninstall the app | Use "Clear All Data" in Settings, or uninstall the app |
| **Google Drive backup** | Retained in your Google Drive until you manually delete it | Delete from your Google Drive or use the app's backup management |
| **Firebase Auth session** | Active until you sign out | Sign out from Settings |
| **Crashlytics data** | Google's standard retention (90 days) | Managed by Google per their data retention policies |
| **SharedPreferences** | Until app is uninstalled or data is cleared | Uninstall or clear app data from device settings |

---

## 10. Your Rights

As a user, you have the following rights regarding your data:

### 10.1 Right to Access
- You can view all your routine data, insights, and profile information directly within the app.
- You can **export your data** as a CSV file from the Settings screen.

### 10.2 Right to Rectification
- You can edit or update your routines, categories, tags, reflections, and profile information at any time.

### 10.3 Right to Deletion
- You can delete individual routines, categories, tags, and reflections from within the app.
- You can use **"Clear All Data"** in Settings to erase all local data and reset the app.
- You can **uninstall the app** to remove all locally stored data from your device.
- You can **sign out** to disconnect your Google account.
- You can **delete your Google Drive backup** directly from Google Drive.

### 10.4 Right to Data Portability
- You can export your data as a **CSV file** for use with other applications.
- You can backup your data to **Google Drive** in a portable JSON format.

### 10.5 Right to Withdraw Consent
- You can revoke Google Sign-In access at any time by signing out.
- You can revoke Google Drive access from your [Google Account Permissions](https://myaccount.google.com/permissions).
- You can deny or revoke any runtime permissions (Camera, Notifications) from your device settings.

---

## 11. Children's Privacy

Aksha is **not directed at children under the age of 13**. We do not knowingly collect personal information from children under 13. If you are a parent or guardian and you believe your child has provided us with personal data, please contact us at the email address listed below, and we will take steps to delete such information.

---

## 12. Offline Functionality

Aksha is designed to work **fully offline**. The core features — creating routines, tracking daily activities, viewing insights, and reflections — do **not** require an internet connection. Internet access is only needed for:

- Google Sign-In (one-time authentication)
- Google Drive backup and restore (user-initiated)
- Firebase Crashlytics (automatic crash reporting)

---

## 13. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. When we make changes:

- The **"Last Updated"** date at the top of this document will be revised.
- For significant changes, we will provide notice within the app (e.g., a dialog or a banner on the Settings screen).
- Continued use of the app after changes constitutes acceptance of the updated policy.

We encourage you to review this Privacy Policy periodically.

---

## 14. Governing Law

This Privacy Policy is governed by the laws of **India**. Any disputes arising out of or in connection with this Privacy Policy shall be subject to the exclusive jurisdiction of the courts in India.

---

## 15. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy or our data practices, please contact us:

- **Email:** bamniyaaakash958@gmail.com
- **Subject Line:** Aksha Privacy Policy Enquiry

We will respond to your enquiry within **30 business days**.

---

## 16. Consent

By downloading, installing, and using Aksha, you consent to the collection and use of your information as described in this Privacy Policy.

---

*This Privacy Policy is specific to the Aksha app (package: `aashu.aksha`) distributed via the Indus App Store and other authorised distribution channels.*



