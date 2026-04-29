# Privacy Policy — MachCrit Logbook

**Last Updated:** April 29, 2026
**Effective Date:** April 29, 2026

---

MachCrit Logbook ("the App", "we", "our") is developed and maintained by **Chad Clarke** as an independent iOS application. This Privacy Policy explains what information the App collects, how it is used and protected, when (if ever) it leaves your device, and what choices you have as a user.

Please read this policy carefully. By using the App you acknowledge that you have read and understood it.

**Contact:** chadclarke1@gmail.com

---

## 1. Overview

MachCrit Logbook is a pilot's flight logbook designed to operate primarily on-device. It has no user accounts, no registration process, and no backend servers operated by the developer. All data you enter is stored locally on your device and, if you choose, optionally synced to your own iCloud account or backed up to a cloud storage provider of your choice.

The App does not sell, rent, or trade your personal information to any third party.

---

## 2. Information We Collect

### 2.1 Location Data

**What is collected:**
When you start a flight recording, the App uses your device's GPS to capture continuous location data: latitude, longitude, altitude, speed, heading, and timestamp. These points form your flight track. Outside of active recording, the App may use low-power significant-location monitoring to detect when a potential flight begins.

**Why it is collected:**
- To record accurate flight tracks for your logbook
- To auto-detect takeoff and landing times
- To calculate flight duration, distance, average speed, and maximum altitude
- To enrich completed flights with ADS-B airport data (Pro feature, opt-in — see Section 3)

**Where it is stored:**
Track points are stored in an encrypted local database on your device. If you have enabled iCloud Sync, track points are included in the data synced to your iCloud account (encrypted end-to-end by Apple).

**Permissions required:**
- "Always" location access (for background flight detection and continuous track capture)
- Precise location access (requested once at the start of your first recording)

You can revoke location permissions at any time in **iOS Settings > Privacy & Security > Location Services > MachCrit Logbook**. Revoking location access will disable flight auto-detection and track recording.

---

### 2.2 Pilot Profile & Credentials

**What is collected:**
Information you voluntarily enter into your pilot profile, including:
- First and last name
- Certificate type (Private Pilot, Commercial, ATP, etc.) and certificate number
- Medical class and expiry date
- Flight review (BFR) expiry date
- Instrument rating expiry
- Class ratings, limitations, and privileges
- Nationality, country, and region
- Optionally: gender, language proficiency

**Why it is collected:**
To display your currency status (medical, BFR), pre-fill logbook fields, and personalise the App to your certificate level.

**Where it is stored:**
Locally on your device in an encrypted database. If iCloud Sync is enabled, this data is synced to your iCloud account (encrypted end-to-end by Apple). This information is never transmitted to MachCrit or any third party.

---

### 2.3 Flight Records

**What is collected:**
Every flight you log or that is auto-recorded, including:
- Date, departure airport, and arrival airport
- Route description and remarks (may be entered by voice — see Section 2.6)
- Takeoff and landing times; block-off and block-on times; duty start and stop times
- Flight hours breakdown: total time, PIC, SIC, dual received, cross-country, actual instrument, simulated instrument, night
- Day and night landing counts; instrument approach count; holds count
- Flight conditions (VFR/IFR/MVFR/LIFR)
- Pilot in Command name, Second in Command (SIC) name, instructor name
- Aircraft assigned to the flight
- Amendment history and audit notes

**Why it is collected:**
To maintain your official pilot logbook record, support regulatory currency tracking, and generate reports.

**Where it is stored:**
Locally on your device in an encrypted database. Optionally synced to iCloud. Never transmitted to MachCrit servers.

---

### 2.4 Aircraft Records

**What is collected:**
Aircraft you add to your logbook, including:
- Registration (tail number)
- Make, model, and year
- Category and class (e.g., SEL, MEL)
- Engine type and performance attributes (complex, high-performance, turbocharged, pressurised, etc.)
- User-entered notes

**Why it is collected:**
To associate aircraft with flight records and support currency and endorsement tracking.

**Where it is stored:**
Locally on your device. Optionally synced to iCloud. Never transmitted to MachCrit servers.

---

### 2.5 Scheduled Flights & Crew

**What is collected:**
If you use the scheduling features:
- Callsign, departure and arrival airports, scheduled date, estimated duration
- Crew member names and their roles (Captain, First Officer, etc.)
- Flight notes and status

**Why it is collected:**
To plan and track upcoming flights and optionally sync them to Apple Calendar.

**Where it is stored:**
Locally on your device. Optionally synced to iCloud and/or Apple Calendar (see Section 2.8).

---

### 2.6 Voice Dictation (Microphone)

**What is collected:**
If you use voice dictation to enter flight remarks, the App captures audio from your device's microphone solely for the purpose of transcription. Transcription is performed **on your device** using Apple's Speech Recognition framework (SFSpeechRecognizer). No audio is recorded, stored, or transmitted externally.

**What is stored:**
Only the resulting plain text (what was transcribed). No audio file is retained.

**Permissions required:**
- Microphone access
- Speech Recognition access

You can revoke these permissions in **iOS Settings > Privacy & Security**. Revoking them disables voice dictation; all other App functions continue normally.

---

### 2.7 Client Information

**What is collected:**
If you use the invoicing and billing features, you may enter client details:
- Company name, contact name, email address, phone number, and mailing address

**Why it is collected:**
To generate flight invoices.

**Where it is stored:**
Locally on your device. Optionally synced to iCloud. Never transmitted to MachCrit servers.

---

### 2.8 Calendar Data

**What is collected:**
If you enable Calendar Sync in Settings, the App reads and writes events to your Apple Calendar. Events contain scheduled flight details: callsign, departure and arrival airports, crew names, aircraft tail number, and notes.

**Why it is collected:**
To provide bidirectional scheduling between MachCrit Logbook and your system calendar.

**Where it is stored:**
In your Apple Calendar on-device. If your device is set up with iCloud Calendar, Apple handles the sync (encrypted end-to-end).

**Permissions required:**
Full Calendar access. Calendar sync is **off by default** and can be disabled in **Settings > Display & Units**.

---

### 2.9 Subscription Status

**What is collected:**
The App checks whether you hold an active Pro subscription via Apple's StoreKit 2 framework. The App stores only a boolean flag ("is subscribed: yes/no") locally.

**What we never see:**
Your Apple ID, payment method, billing address, or transaction receipts. All subscription management, billing, and receipt validation is handled entirely by Apple.

**Subscription products:**
- MachCrit Pro Monthly (`com.cwr.MachCrit.pro.monthly`)
- MachCrit Pro Annual (`com.cwr.MachCrit.pro.annual`)

---

### 2.10 Device Identifier

**What is collected:**
A randomly generated device identifier (UUID) is created the first time you install the App on a device and stored in the iOS Keychain. It persists across app reinstalls on the same hardware.

**Why it is collected:**
Solely for sync conflict resolution when the same data is edited on multiple devices. When two devices both modify the same flight record, the device ID is used as a tiebreaker to determine which change wins.

**Where it is stored:**
In the iOS Keychain on your device only. It is never transmitted to MachCrit servers or any third party. It is included in iCloud sync metadata only to the extent that Apple's CloudKit framework uses it internally for change tracking.

---

## 3. ADS-B Enrichment (Pro Feature — Opt-In)

MachCrit Logbook includes an optional Pro feature that attempts to match your completed flight against public ADS-B flight data provided by FlightRadar24 (FR24). This can automatically fill in departure and arrival airports when they were not recorded.

**What data leaves your device when this feature is active:**

| Data sent | Purpose |
|---|---|
| Aircraft registration (tail number) | Match your flight against FR24's ADS-B records by registration |
| Flight time window (takeoff ± 5 minutes, landing ± 5 minutes) | Narrow the search to your specific flight |
| GPS bounding box (min/max lat/lon ± ~6 NM) | Used only if no aircraft is selected; finds flights in the area |

**What is NOT sent:**
Pilot name, certificate, hours, remarks, crew names, medical status, or any other personal information.

**How the request is routed:**
All queries go through a Cloudflare Worker proxy operated by the developer. The proxy validates the request, then forwards it to FlightRadar24's REST API. The proxy does not log query content or personal data. FlightRadar24's own privacy policy governs how they handle the incoming request (aircraft registration, time window, and IP address of the proxy).

**This feature is:**
- Disabled by default
- Requires a Pro subscription
- Can be turned off at any time in **Settings > ADS-B Enhancement**

---

## 4. Data Storage & Security

### On-Device Storage
- The Core Data database is protected with **NSFileProtectionComplete**, which means it is encrypted while the device is locked and inaccessible to other apps.
- Automatic backups are encrypted with **AES-256-GCM** before being written to disk. The encryption key is generated by the App and stored in the iOS Keychain (system-managed, non-exportable).

### iCloud Sync
- If enabled, your data is synced via Apple's CloudKit service. Apple encrypts this data end-to-end. The developer has no access to your iCloud data.
- You can disable iCloud sync for the App in **iOS Settings > [Your Name] > iCloud > MachCrit Logbook**.

### Cloud Backups (Optional)
- You may configure the App to store encrypted backups in iCloud Drive, Dropbox, OneDrive, or Google Drive.
- Backups are encrypted with AES-256-GCM **before** they leave your device. The cloud storage provider receives only an encrypted binary file — they cannot read its contents.
- The encryption passphrase is stored in iCloud Keychain (accessible across your devices) and as a fallback in the local device Keychain.

### Audit Trail
- The App maintains an append-only, tamper-detected change history for all flights, aircraft, and settings. Each entry is linked with a cryptographic hash chain to detect unauthorized modification.
- The audit trail is stored locally (and in iCloud if sync is enabled). It is never transmitted to MachCrit.

### No Backend Servers
The developer does not operate any backend servers that store your data. There are no MachCrit user accounts. All data belongs to you and lives under your control (on your device and in your iCloud account).

---

## 5. Data Sharing

We do not sell, rent, trade, or otherwise share your personal information with third parties for their own purposes. The only disclosures of your data are:

| Recipient | What is shared | When | Your control |
|---|---|---|---|
| **Apple (iCloud/CloudKit)** | All app data | If iCloud Sync is enabled | Toggle in iOS Settings |
| **FlightRadar24** (via Cloudflare proxy) | Aircraft registration + time window or GPS bounding box | If ADS-B Enrichment is enabled (Pro) | Toggle in App Settings |
| **Apple Calendar** | Scheduled flight details | If Calendar Sync is enabled | Toggle in App Settings |
| **Cloud storage providers** (iCloud Drive, Dropbox, OneDrive, Google Drive) | AES-encrypted backup blob | If Cloud Backup is configured | Configure in App Settings |
| **Apple (StoreKit)** | Subscription purchase interaction | When purchasing Pro | Managed by Apple |

---

## 6. Analytics & Advertising

MachCrit Logbook contains **no third-party analytics SDKs** (such as Firebase Analytics, Mixpanel, or Amplitude), **no advertising SDKs**, and **no crash-reporting services** (such as Crashlytics or Sentry). The App does not track you across other apps or websites.

---

## 7. Your Rights & Choices

**Access your data:** All your data is visible within the App at all times. You may also export a full encrypted backup via **Settings > Data & Integrity > Back Up Now**.

**Delete your data:** You may delete individual flights or aircraft from within the App. Deleting the App removes all local data. To remove data from iCloud, visit icloud.com and manage the App's container, or disable iCloud sync before deleting the App.

**Withdraw permissions:** You may revoke location, microphone, speech recognition, and calendar permissions at any time in **iOS Settings > Privacy & Security**. Revoking a permission disables the related feature but does not affect data already stored.

**Opt out of enrichment:** You may disable ADS-B Enrichment at any time in **Settings > ADS-B Enhancement**.

**Opt out of iCloud Sync:** Toggle off in **iOS Settings > [Your Name] > iCloud > MachCrit Logbook**.

**Portability:** Your data can be exported as an encrypted backup at any time from the App's Settings screen.

---

## 8. Data Retention

The App retains your data for as long as you use it. There is no automatic expiry. If you delete the App, all local data is removed. iCloud data persists until you remove it manually via iCloud.com or the App's backup restore feature.

The App's audit trail is append-only by design (it cannot be selectively deleted). This is a data integrity feature, not a retention policy imposed by the developer. You can clear the entire audit trail by importing a fresh backup that pre-dates the events you wish to remove.

---

## 9. Children's Privacy

MachCrit Logbook is not directed at children under the age of 13, and we do not knowingly collect personal information from children under 13. If you are a parent or guardian and believe your child has provided personal information through the App, please contact us so we can remove it.

---

## 10. International Users

MachCrit Logbook is developed in South Africa and available globally. If you are located in the European Economic Area (EEA), United Kingdom, or another jurisdiction with privacy regulations, the following applies:

- **Legal basis for processing:** Your data is processed on the basis of your consent (granting permissions) and the performance of a contract (providing the logbook service you requested).
- **Your rights under GDPR / UK GDPR:** You have the right to access, rectify, erase, restrict processing of, and obtain a portable copy of your personal data. To exercise these rights, contact us at chadclarke1@gmail.com. Since no data is stored on MachCrit servers, most of these rights are exercised directly within the App or through iCloud settings.
- **Data transfers:** If iCloud Sync or cloud backup is enabled, your data is transferred to Apple's or your chosen provider's servers, which may be located outside your home jurisdiction. Apple complies with applicable international data transfer requirements.

---

## 11. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will update the "Last Updated" date at the top of this page. Material changes will be noted in the App's release notes. Your continued use of the App after a change constitutes your acceptance of the revised policy.

The version history of this policy is available in the Git repository where it is maintained.

---

## 12. Contact

If you have questions, concerns, or requests regarding this Privacy Policy or your data:

**Chad Clarke**
Email: chadclarke1@gmail.com

---

*This policy covers MachCrit Logbook for iOS. It does not cover third-party services such as Apple iCloud, FlightRadar24, Dropbox, OneDrive, or Google Drive, each of which has its own privacy policy.*
