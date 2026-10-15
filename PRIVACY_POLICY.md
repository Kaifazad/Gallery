# Privacy Policy for Gallery

**Effective Date:** October 15, 2026  
**Application Name:** Gallery  
**Package Name:** `com.kaifazad.gallery`  
**Developer:** Kaif Azad  
**GitHub Repository:** [https://github.com/Kaifazad/Gallery](https://github.com/Kaifazad/Gallery)  

---

### 1. Introduction & Core Philosophy
Thank you for using **Gallery**. We believe that your personal photos, videos, and memories belong exclusively to you.

Gallery is built from the ground up as a **100% offline, privacy-first media gallery**. The application operates entirely locally on your device. We do not collect, transmit, sell, or monitor your personal information, photos, videos, or device usage under any circumstances.

---

### 2. Zero Internet Permission (100% Offline)
Gallery has **no network access**. The application's Android manifest explicitly removes all internet and network permissions:
- `android.permission.INTERNET` — **Removed**
- `android.permission.ACCESS_NETWORK_STATE` — **Removed**
- `android.permission.ACCESS_WIFI_STATE` — **Removed**

Because the application lacks network capabilities, it is technically impossible for Gallery to transmit your photos, videos, or metadata to external servers, cloud providers, or third parties.

---

### 3. Data Collection & Analytics
- **Personal Data:** We collect **zero** personal information (no names, email addresses, phone numbers, contacts, or accounts).
- **Media & Files:** Your photos and videos remain stored locally on your device. We do not upload, copy, or sync your media anywhere.
- **Analytics & Telemetry:** Gallery contains **zero trackers, zero analytics SDKs, and zero telemetry**. We do not use Google Analytics, Firebase, Crashlytics, or any third-party tracking libraries.
- **Advertisements:** Gallery contains **no ads** and no advertising frameworks.

---

### 4. Device Permissions & How They Are Used
Gallery requests only the permissions necessary to function as a full-featured on-device media manager:

| Permission | Purpose |
| :--- | :--- |
| `READ_MEDIA_IMAGES` / `READ_MEDIA_VIDEO` | Required on Android 13+ to discover, display, and organize your local photos and videos through Android's standard Scoped MediaStore. |
| `READ_EXTERNAL_STORAGE` / `WRITE_EXTERNAL_STORAGE` | Used on Android 10 and below for local media access. |
| `ACCESS_MEDIA_LOCATION` | Allows you to view EXIF geographical metadata (latitude, longitude, altitude) locally within the media inspector. This data never leaves your device. |
| `MANAGE_MEDIA` *(Optional)* | Allows seamless photo management and trashing on Android 12+ without prompting system confirmation popups for every single action. |
| `POST_NOTIFICATIONS` | Used solely to display local progress indicators during bulk media operations (such as encrypting or decrypting media in the Vault). |
| `VIBRATE` | Direct hardware tactile feedback for touch interactions and navigation. |

---

### 5. Encrypted Vault Security
The built-in **Vault** feature allows you to secure sensitive media behind biometric authentication or a custom password.
- **Encryption Standard:** Vault items are encrypted at rest using industry-standard **AES-256 GCM** encryption.
- **Key Storage:** Encryption keys are protected locally on your device using the Android Keystore system.
- **Isolation:** Vaulted files are hidden from system indexing, external applications, and media scanners.

---

### 6. Third-Party Interactions
- When you explicitly choose to share a photo or video (via the Android system share sheet) or choose to edit an image with an external editor, Gallery invokes standard Android system intents to hand off the file URI to your selected app.
- When opening GPS coordinates in external maps, Gallery sends a geo-intent to your default map provider (e.g., Google Maps, OpenStreetMap).

---

### 7. Children's Privacy (COPPA Compliance)
Gallery does not collect, store, or solicit any personal information from anyone, including children under the age of 13.

---

### 8. Changes to This Privacy Policy
We may update this policy if new local features are introduced. Any updates will always maintain our zero-data-collection standard and will be published directly in this repository.

---

### 9. Contact
If you have any questions, feedback, or concerns regarding this Privacy Policy:
- **Developer:** Kaif Azad
- **Email:** itzkaifazad@gmail.com
- **GitHub:** [https://github.com/Kaifazad/Gallery](https://github.com/Kaifazad/Gallery)
- **Instagram:** [https://instagram.com/kaif.azad](https://instagram.com/kaif.azad)
