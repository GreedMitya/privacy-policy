# Data Deletion Instructions — Glazd

**App:** Glazd — Anonymous Interest Matching  
**Developer:** GreedMitya  
**Contact:** [senseimitya@gmail.com]

---

## How to Delete Your Account and Data

Google Play requires all apps with accounts to provide a clear data deletion path. Here is how to delete your Glazd account and all associated data.

---

## Option 1: Delete from Within the App (Recommended)

This is the fastest and most complete method.

1. Open **Glazd**
2. Tap **Profile** tab (bottom navigation)
3. Tap **Settings** (gear icon)
4. Scroll to the bottom and tap **Delete Account**
5. Confirm the deletion in the dialog

**What happens immediately:**
- ✅ Your Firebase authentication record is deleted (phone number association removed)
- ✅ Your user profile is permanently deleted
- ✅ Your interest vector and computed category scores are deleted
- ✅ All match scores involving your account are deleted
- ✅ All chats you participated in are deleted (including all messages)
- ✅ All pending and past chat requests are deleted
- ✅ Your push notification token is removed

**This is irreversible.** There is no grace period — deletion is immediate and permanent.

---

## Option 2: Submit a Deletion Request by Email

If you cannot access the app (e.g. lost your phone), you can submit a deletion request:

📧 **Email:** [senseimitya@gmail.com]  
**Subject:** Data Deletion Request — Glazd  
**Include:** The phone number associated with your account (in +48XXXXXXXXX format)

We will process your request within **30 days** and confirm deletion by reply email.

---

## What Data Is Deleted

| Data | Deleted? | Notes |
|------|----------|-------|
| Phone number (Firebase Auth) | ✅ Yes | Authentication record fully removed |
| TikTok username | ✅ Yes | Was stored privately; removed |
| Display name | ✅ Yes | |
| Interest vector (category scores) | ✅ Yes | |
| Avatar configuration | ✅ Yes | |
| Vibe label | ✅ Yes | |
| Match scores with other users | ✅ Yes | Pair records deleted |
| Chat messages | ✅ Yes | All messages in all chats |
| Chat documents | ✅ Yes | |
| Chat requests (sent and received) | ✅ Yes | |
| FCM push token | ✅ Yes | |
| TikTok data export file (raw JSON) | ✅ Already deleted | Deleted automatically within seconds of original upload |

---

## Note on Firebase Analytics / Crashlytics

Anonymized crash and analytics events may be retained by Google Firebase for up to 14 months per Google's data retention policy. These events are not linked to your identity after account deletion.

---

## Questions?

Contact: **[senseimitya@gmail.com]**

Response time: Within 30 days (GDPR requirement).

---

*This page is part of the Glazd legal documentation. See also: [Privacy Policy](glazd.md) | [Terms of Service](glazd-terms.md)*
