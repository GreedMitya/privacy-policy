# Privacy Policy — Glazd

**Effective Date:** March 2026  
**Last Updated:** March 2026  
**Developer:** GreedMitya (operating under personal name)  
**Contact:** [senseimitya@gmail.com]  
**Firebase Data Region:** europe-central2 (Warsaw, EU)

---

## 1. Introduction

Glazd ("the App", "we", "us") is an anonymous interest-matching social application for Android. We match users based on shared TikTok content interests, without requiring real names, photos, or personal social profiles.

This Privacy Policy explains what data we collect, how we use it, and your rights under the **General Data Protection Regulation (GDPR)** and Polish data protection law (**RODO**).

By using Glazd, you agree to the practices described in this policy. Your use of the App is also governed by our [Terms of Service](terms_of_service.md). If you disagree with this policy or our Terms, please do not use the App.

---

## 2. Data We Collect

### 2.1 Data You Provide Directly

| Data | Purpose | Visibility to Other Users |
|------|---------|--------------------------|
| **Phone number** | One-time authentication via SMS OTP (Firebase Auth) | 🔒 Never visible to other users |
| **Email address** | Support requests and account management | 🔒 Never visible to other users |
| **TikTok username** | Bot-prevention identity verification | 🔒 Never visible to other users |
| **Display name** | Your anonymous in-app name (you choose it) | ✅ Visible (e.g. "CosyReader42") |
| **Optional bio** (max 200 chars) | Brief self-description (Personalization) | ✅ Visible if provided |
| **Age range** (18-24, 25-30, 31+) | Displayed on profile (Personalization) | ✅ Visible if provided |
| **City** (default: Warsaw) | Discover feature (Personalization) | ✅ Visible |

### 2.2 TikTok Data Export (Core Feature)

To use Glazd, you upload a **TikTok data export file** (a `.json` file you download from TikTok's own settings). This file is processed by our servers to compute your interest profile.

> **Critical privacy fact:** The raw TikTok data export file is **automatically and permanently deleted** from our servers within seconds of being processed. We never store it, and no human ever reads it. Only the computed interest scores (anonymized numbers) are retained.

What we extract from the export:
- Watch and like history → to identify content categories you enjoy
- Search terms → to understand active interests
- Hashtags engaged with → to refine category scoring
- Profile bio → high-confidence self-description

What we **do not** extract or store:
- Your TikTok follower list
- Your TikTok DMs or comments
- Any identifiable TikTok video IDs after processing

### 2.3 Data We Generate Automatically

| Data | Description | Visibility |
|------|-------------|------------|
| **Interest vector** | ~60 category scores (Personalization) | 🔒 Never shown raw to others |
| **Vibe label** | Auto-generated label (Personalization) | ✅ Shown to chat partners |
| **Interest avatar** | Auto-generated icon + color (Personalization) | ✅ Shown in Discover list |
| **Match scores** | Cosine similarity score (App functionality) | ✅ Shown as "85% match" |
| **Presence status** | Online / Offline + last seen (App functionality) | ✅ Online indicator shown |
| **FCM/Device IDs** | Firebase UID, FCM tokens, Android ID (Diagnostics) | 🔒 Internal use only |

### 2.4 Usage Data

- **Chat messages**: Text/media messages you send (App functionality). Stored in encrypted form. Visible only to you and your chat partner.
- **Reports**: Content stored for moderation review (App functionality).
- **App activity & Diagnostics**: Clicks, screen views, and crash reports (Firebase Analytics & Crashlytics). Purpose: Analytics.

---

## 3. How We Use Your Data

| Purpose | Legal Basis (GDPR) |
|---------|-------------------|
| Authenticate your identity (phone OTP) | Account management |
| Verify you're a real TikTok user | Account management |
| Compute your interest profile | Personalization |
| Match you with other users | App functionality |
| Display public profile | App functionality |
| Send push notifications | App functionality |
| Moderate content and safety | App functionality |
| Improve and fix the app (Firebase Crashlytics) | Analytics |
| Analyze app usage (Firebase Analytics) | Analytics |

We do **not** use your data for advertising. We do **not** build advertising profiles. We do **not** sell your data to any third party.

---

## 4. What Other Users Can See

Glazd is designed with **anonymity as a core feature**. Here is a precise breakdown:

**Other users CAN see:**
- Your display name (chosen by you — does not need to be your real name)
- Your automatically generated interest avatar (icon + color)
- Your top interest categories and match percentages
- Your online/offline status and approximate last-seen time
- Your optional bio, age range, and city (if provided)
- Messages you send them after a chat is started

**Other users CANNOT see:**
- Your phone number
- Your TikTok username
- Your raw TikTok data export or any raw interest data
- Exact session start or end times
- Your Firebase UID directly

These restrictions are enforced at the server level through **Firestore security rules** and **Cloud Function validation** — not just in the app interface. Clients cannot bypass them.

---

## 5. Data Sharing and Third Parties

We use the following infrastructure providers:

| Provider | Purpose | Privacy Policy |
|----------|---------|---------------|
| **Google Firebase** (Auth, Firestore, Storage, Functions, FCM, Analytics, Crashlytics) | Core app infrastructure | [firebase.google.com/support/privacy](https://firebase.google.com/support/privacy) |

All Firebase data is stored in **europe-central2 (Warsaw, EU)** and does not leave the European Union.

We do **not** share your personal data with:
- Advertisers or marketing platforms
- Data brokers
- Other app developers
- Any other third parties

---

## 6. Data Retention

| Data | Retention Period |
|------|----------------|
| TikTok data export file (raw JSON) | **Deleted within seconds** of processing |
| Interest vector (computed categories) | Until account is deleted |
| User profile (display name, avatar, etc.) | Until account is deleted |
| Chat messages | Until the chat is deleted by either participant |
| Match scores | Until either user's account is deleted |
| Push tokens | Until account is deleted or token refreshed |
| Reports | 90 days after resolution, then deleted |
| Firebase Analytics / Crashlytics | Per Google's retention policy (up to 14 months) |

---

## 7. Account Deletion

You can **permanently delete your account** at any time from within the app (Profile → Settings → Delete Account).

Upon deletion, we immediately and permanently remove:
- Your user profile document
- Your interest vector
- All match scores involving your account
- All chats you participated in (including messages)
- All pending or past chat requests
- Your Firebase Auth record (phone number association)

This deletion is irreversible and automatic. No support request is needed.

---

## 8. Your Rights Under GDPR / RODO

As a user in the European Union, you have the following rights:

- **Right of access** — You can request a copy of all personal data we hold about you.
- **Right to rectification** — You can update your profile data directly in the app, or request corrections.
- **Right to erasure ("right to be forgotten")** — Delete your account in-app at any time for full, immediate deletion.
- **Right to data portability** — You can request an export of your personal data in JSON format by emailing us at the address provided below.
- **Right to restrict processing** — You can request that we limit how we use your data while a dispute is investigated.
- **Right to object** — You can object to processing based on legitimate interest.
- **Right to lodge a complaint** — You have the right to file a complaint with the Polish Data Protection Authority (UODO): [uodo.gov.pl](https://uodo.gov.pl)

To exercise any rights (other than account deletion, which is in-app), contact: **[senseimitya@gmail.com]**

We will respond within **30 days**.

---

## 9. Children's Policy

Glazd is intended for users **18 years of age and older**. We do not knowingly collect data from anyone under 18. We strictly adhere to our [Child Safety Standards](child_safety_standards.md). If you believe a minor has created an account, please contact us at **[senseimitya@gmail.com]** and we will delete it promptly.

---

## 10. Security

- **In transit**: All data is encrypted using TLS (HTTPS).
- **At rest**: All Firestore and Cloud Storage data is encrypted using AES-256 (Google default).
- **Access control**: Sensitive fields (phone number, TikTok username) are protected by Firestore security rules — no client query can access them.
- **Rate limiting**: The app enforces server-side rate limits (20 chat requests/hour, 60 messages/hour) to prevent abuse.
- **Moderation**: Users can report others. Accounts receiving 5 reports are automatically reviewed and may be banned.

---

## 11. Push Notifications

We use **Firebase Cloud Messaging (FCM)** to deliver notifications about chat requests and messages.

- Notifications are sent only for in-app events (not promotional).
- You can disable notifications at any time in your device settings (Android → Apps → Glazd → Notifications).

---

## 12. Changes to This Policy

We may update this Privacy Policy from time to time. Material changes will be communicated via an in-app notification. The "Last Updated" date at the top of this page will always reflect the current version.

Continued use of the app after changes constitutes acceptance of the updated policy.

---

## 13. Contact

**Data Controller:**  
GreedMitya  
[Poznan, Poland]  
Email: **[senseimitya@gmail.com]**

For GDPR/RODO data requests, please include "Data Request — Glazd" in the subject line.

---

*Glazd is developed independently as a personal project. Firebase is a service of Google LLC.*
