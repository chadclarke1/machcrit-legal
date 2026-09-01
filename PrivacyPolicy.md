# Privacy Policy — MachCrit Logbook

**Last Updated:** September 1, 2026  
**Effective Date:** September 1, 2026  
**Applies to:** MachCrit for iPhone, iPad, and Apple silicon Mac (App Store version 1.95 and later)

---

MachCrit Logbook ("the App", "we", "our") is developed and maintained by **Chad Clarke** as an independent Apple application. This Privacy Policy explains what information the App collects, how it is used and protected, when (if ever) it leaves your device, and what choices you have as a user.

Please read this policy carefully. By using the App you acknowledge that you have read and understood it.

**Contact:** chadclarke1@gmail.com

**Summary of this update:** This policy has been revised to match the current App, including Pilot Wallet credentials, Smart Assist and document-assisted import, App Lock, airport records, reports and exports, Apple Maps display, Family Sharing, and South African POPIA disclosures. The on-device, no-account model is unchanged.

---

## 1. Overview

MachCrit is a pilot's personal logbook designed to operate primarily on-device. It has no user accounts, no registration process, and no MachCrit servers that store your logbook. All data you enter is stored locally on your device and, if you choose, optionally synced to your own iCloud account or backed up to a cloud storage provider of your choice.

The only developer-operated network service is an optional ADS-B enrichment proxy (see Section 3). That proxy does not create accounts and is not used to store your logbook, credentials, or backups.

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
- To display your track on a map
- To enrich completed flights with ADS-B airport data (Pro feature, opt-in — see Section 3)

**Where it is stored:**
Track points are stored in an encrypted local database on your device. If you have enabled iCloud Sync, track points are included in the data synced to your iCloud account (encrypted end-to-end by Apple).

**Permissions required:**
- "Always" location access (for background flight detection and continuous track capture)
- Precise location access (requested when you first record)

You can revoke location permissions at any time in **iOS / iPadOS / macOS Settings > Privacy & Security > Location Services > MachCrit**. Revoking location access will disable flight auto-detection and track recording. Manual logbook entry continues to work.

---

### 2.2 Pilot Wallet, Profile & Credentials

**What is collected:**
Information you voluntarily enter into your pilot profile and Pilot Wallet, including:
- First and last name
- Certificate or licence type (Private Pilot, Commercial, ATP, CPL, and similar) and certificate or licence number
- Issuing authority and country (for example SACAA, FAA, CASA, CAA)
- Medical class and expiry date
- Flight review, proficiency check, or equivalent expiry dates
- Instrument rating expiry
- Class ratings, limitations, and privileges
- Nationality, country, and region
- Optionally: gender, language proficiency
- Optionally: images or files of physical licences, medical certificates, or other credentials you choose to store in Pilot Wallet

**Why it is collected:**
To display your currency status, pre-fill logbook fields, personalise the App to your certificate level, and keep a convenient on-device record of licences and medicals.

**Where it is stored:**
Locally on your device in an encrypted database. If iCloud Sync is enabled, this data is synced to your iCloud account (encrypted end-to-end by Apple). This information is never transmitted to MachCrit or any third party for MachCrit's own purposes.

Pilot Wallet is a personal convenience display. It is **not** an official digital licence, medical certificate, or credential issued by any aviation authority.

---

### 2.3 Flight Records

**What is collected:**
Every flight you log or that is auto-recorded, including:
- Date, departure airport, and arrival airport
- Route description and remarks (may be entered by voice — see Section 2.7)
- Takeoff and landing times; block-off and block-on times; duty start and stop times
- Flight hours breakdown: total time, PIC, SIC, dual received, instructor, cross-country, actual instrument, simulated instrument, night, and simulator time where used
- Day and night landing counts; instrument approach count; holds count
- Flight conditions (VFR/IFR/MVFR/LIFR)
- Pilot in Command name, Second in Command (SIC) name, instructor name
- Aircraft assigned to the flight
- Custom metadata fields you enable on the Flight Card
- Amendment history and audit notes

**Why it is collected:**
To maintain your personal pilot logbook record, support regulatory currency tracking for supported rule sets, generate reports, and (if you use them) invoices.

**Where it is stored:**
Locally on your device in an encrypted database. Optionally synced to iCloud. Never transmitted to MachCrit servers.

---

### 2.4 Aircraft Records

**What is collected:**
Aircraft you add to your logbook, including:
- Registration (tail number)
- Make, model, and year
- Category and class (for example SEL, MEL, simulator)
- Engine type and performance attributes (complex, high-performance, turbocharged, pressurised, tailwheel, retractable, and similar)
- User-entered notes and status (active, inactive, default, favourite)

**Why it is collected:**
To associate aircraft with flight records and support currency and endorsement tracking.

**Where it is stored:**
Locally on your device. Optionally synced to iCloud. Never transmitted to MachCrit servers.

---

### 2.5 Airport Records

**What is collected:**
Airports, airfields, and heliports you use or add, including:
- ICAO or IATA codes, name, city, country, and coordinates
- Home or base designation
- Notes, usage counts, and matching status against the App's reference airport dataset

**Why it is collected:**
To associate flights with departure and arrival locations, support search and reporting, and help you keep a personal airport list.

**Where it is stored:**
In a local database on your device, together with a bundled or updated reference airport dataset. User-added airports and notes are optionally synced to iCloud. The reference dataset is for convenience only and is not an aeronautical chart or operational airport directory.

---

### 2.6 Scheduled Flights & Crew

**What is collected:**
If you use the scheduling features:
- Callsign, departure and arrival airports, scheduled date, estimated duration
- Crew member names and their roles (Captain, First Officer, and similar)
- Flight notes and status
- Optional schedule-matching data used to associate a scheduled item with a recorded or enriched flight

**Why it is collected:**
To plan and track upcoming flights, optionally sync them to Apple Calendar, and (if enabled) match schedules to completed records.

**Where it is stored:**
Locally on your device. Optionally synced to iCloud and/or Apple Calendar (see Section 2.10).

---

### 2.7 Voice Dictation (Microphone)

**What is collected:**
If you use voice dictation to enter flight remarks, the App captures audio from your device's microphone solely for the purpose of transcription. Transcription is performed **on your device** using Apple's Speech Recognition framework. No audio is recorded, stored, or transmitted by MachCrit.

**What is stored:**
Only the resulting plain text (what was transcribed). No audio file is retained.

**Permissions required:**
- Microphone access
- Speech Recognition access

You can revoke these permissions in **Settings > Privacy & Security**. Revoking them disables voice dictation; all other App functions continue normally.

---

### 2.8 Smart Import, Documents, Camera & Photos

**What is collected:**
If you use smart import or document-assisted workflows (Pro, where available), you may choose to import:
- Logbook files (for example CSV or other supported export formats)
- Photos or scans of paper logbook pages, licences, or related documents
- PDFs or other files you select through the system file picker

The App may use on-device Vision, Optical Character Recognition, and (where available) Apple Intelligence / Foundation Models to propose structured flight, aircraft, or credential fields from that material.

**Why it is collected:**
To reduce manual data entry. Proposed values are suggestions only until you review and save them.

**Where it is stored:**
Extracted text and the resulting logbook records are stored locally (and in iCloud if sync is enabled). Original images or files are stored only if you keep them attached to a record. Imported content is not uploaded to MachCrit servers.

**Permissions that may be requested when you use these features:**
- Camera (to photograph a document)
- Photo Library (to choose an existing image)
- Files / document picker access

These permissions are optional. Declining them disables import-from-camera or import-from-photos; manual entry continues to work.

**What is NOT done:**
MachCrit does not send your documents to a developer-operated AI service, and does not use imported documents to train models for other users.

---

### 2.9 Smart Assist (Pro Feature — Opt-In)

**What it is:**
Smart Assist is an optional Pro feature that can provide on-device assistance such as suggested field values, smart import help, flight-intelligence summaries, and related suggestions. It is **off by default** and can be turned off in **Settings > Enhancements**.

**What data is processed:**
Only the logbook, document, or field context needed for the suggestion you requested — for example a draft flight, imported page, or selected record.

**Where processing happens:**
Assistance is intended to run **on your device** using Apple system frameworks. On supported devices with Apple Intelligence enabled, Apple's on-device Foundation Models may be used. If Apple routes a request through Apple Intelligence Private Cloud Compute, that processing is performed by Apple under [Apple's Privacy Policy](https://www.apple.com/privacy/) and Apple Intelligence terms, not on MachCrit servers.

**What we never see:**
The Developer does not receive your prompts, documents, or Smart Assist outputs.

Smart Assist suggestions are convenience aids. They are not certified aviation data, legal advice, or a substitute for your own verification.

---

### 2.10 Client Information & Invoicing

**What is collected:**
If you use the invoicing and billing features, you may enter client details:
- Company name, contact name, email address, phone number, and mailing address
- Invoice amounts, flight references, and related billing notes

**Why it is collected:**
To generate flight invoices on your device.

**Where it is stored:**
Locally on your device. Optionally synced to iCloud. Never transmitted to MachCrit servers. If you export or share an invoice, the recipient sees whatever you chose to send.

---

### 2.11 Calendar Data

**What is collected:**
If you enable Calendar Sync in Settings, the App reads and writes events to your Apple Calendar. Events contain scheduled flight details: callsign, departure and arrival airports, crew names, aircraft tail number, and notes.

**Why it is collected:**
To provide bidirectional scheduling between MachCrit Logbook and your system calendar.

**Where it is stored:**
In your Apple Calendar on-device. If your device is set up with iCloud Calendar, Apple handles the sync (encrypted end-to-end).

**Permissions required:**
Calendar access. Calendar sync is **off by default** and can be disabled in **Settings > Calendar & Scheduling**.

---

### 2.12 Maps

The Record screen and track review use Apple Maps / MapKit to display geography and your flight track. Map display may cause your device to request map tiles from Apple. Apple may receive the map region being viewed. This is handled by Apple, not by MachCrit servers.

Maps in the App are for reviewing recorded tracks and locating airports in your logbook. They are not certified charts and are not for navigation or in-flight operational use.

---

### 2.13 Reports, Exports & Sharing

You may generate reports and export records (for example PDF, CSV, or encrypted backup) and share them through the system share sheet, AirDrop, Mail, Files, or another app you choose.

**What leaves your device:**
Only the file you explicitly export or share, and only to the destination you select. MachCrit does not upload exports to a MachCrit server.

You are responsible for choosing recipients and for redacting any information you do not wish to share.

---

### 2.14 App Lock & Biometrics

If you enable App Lock, the App uses the device passcode, Face ID, or Touch ID through Apple's Local Authentication framework to gate access to the App.

**What is collected:**
The App stores only a local setting that App Lock is enabled. It does not receive, store, or transmit your biometric templates. Face ID and Touch ID data remain in the Secure Enclave and are never available to MachCrit.

You can disable App Lock in Settings. You can also revoke Face ID / Touch ID access for the App in system Settings.

---

### 2.15 Subscription Status

**What is collected:**
The App checks whether you hold an active Pro subscription via Apple's StoreKit 2 framework. The App stores only a local entitlement state (subscribed or not, and related StoreKit transaction metadata required to unlock Pro features).

**What we never see:**
Your Apple ID, payment method, billing address, or full payment receipts. All subscription management, billing, and receipt validation is handled entirely by Apple.

**Subscription products:**
- MachCrit Pro Monthly (`com.cwr.MachCrit.pro.monthly`)
- MachCrit Pro Annual (`com.cwr.MachCrit.pro.annual`)

If Family Sharing is enabled on your Apple ID, a Pro subscription may be shared with your Family Sharing group according to Apple's rules. The Developer does not manage Family Sharing.

---

### 2.16 Device Identifier

**What is collected:**
A randomly generated device identifier (UUID) is created the first time you install the App on a device and stored in the iOS / iPadOS / macOS Keychain. It persists across app reinstalls on the same hardware.

**Why it is collected:**
Solely for sync conflict resolution when the same data is edited on multiple devices. When two devices both modify the same record, the device ID is used as a tiebreaker to determine which change wins.

**Where it is stored:**
In the device Keychain only. It is never transmitted to MachCrit servers or any third party. It is included in iCloud sync metadata only to the extent that Apple's CloudKit framework uses it internally for change tracking.

---

### 2.17 On-Device Diagnostics

**Settings > Advanced Features** may include developer diagnostics and troubleshooting tools. Diagnostic logs are generated on your device to help you (or, if you choose, the Developer) diagnose a problem.

Diagnostics are not sent automatically. They are not processed by Crashlytics, Sentry, or any other third-party crash service. If you contact support, you may optionally attach a diagnostic export; only then would the Developer see the content you chose to send.

---

## 3. ADS-B Enrichment (Pro Feature — Opt-In)

MachCrit Logbook includes an optional Pro feature that attempts to match your completed flight against public ADS-B flight data provided by FlightRadar24 (FR24). This can automatically fill in departure and arrival airports, callsigns, or supplemental track points when they were not recorded.

**What data leaves your device when this feature is active:**

| Data sent | Purpose |
|---|---|
| Aircraft registration (tail number) | Match your flight against FR24's ADS-B records by registration |
| Flight time window (takeoff ± 5 minutes, landing ± 5 minutes) | Narrow the search to your specific flight |
| GPS bounding box (min/max lat/lon ± ~6 NM) | Used only if no aircraft is selected; finds flights in the area |

**What is NOT sent:**
Pilot name, licence or certificate numbers, hours, remarks, crew names, medical status, Pilot Wallet contents, imported documents, invoices, or any other personal information.

**How the request is routed:**
All queries go through a Cloudflare Worker proxy operated by the developer. The proxy validates the request, then forwards it to FlightRadar24's REST API. The proxy does not store your logbook and is not intended to log query content or personal data. FlightRadar24's own privacy policy governs how they handle the incoming request (aircraft registration, time window, and IP address of the proxy).

This proxy is the only developer-operated network component. It does not provide user accounts and does not hold your Core Data store, backups, or credentials.

**This feature is:**
- Disabled by default
- Requires a Pro subscription
- Can be turned off at any time in **Settings > Enhancements** (ADS-B / schedule matching)

---

## 4. Data Storage & Security

### On-Device Storage
- The Core Data database is protected with **NSFileProtectionComplete** (or the platform equivalent), which means it is encrypted while the device is locked and inaccessible to other apps.
- Automatic backups are encrypted with **AES-256-GCM** before being written to disk. The encryption key is generated by the App and stored in the device Keychain (system-managed, non-exportable).
- Optional App Lock adds an additional local gate using the system passcode or biometrics.

### iCloud Sync
- If enabled, your data is synced via Apple's CloudKit service. Apple encrypts this data end-to-end. The developer has no access to your iCloud data.
- You can disable iCloud sync for the App in system Settings under iCloud, or from **Settings > Data & Cloud** in the App where that control is provided.

### Cloud Backups (Optional)
- You may configure the App to store encrypted backups in iCloud Drive, Dropbox, OneDrive, or Google Drive.
- Backups are encrypted with AES-256-GCM **before** they leave your device. The cloud storage provider receives only an encrypted binary file — they cannot read its contents.
- The encryption passphrase is stored in iCloud Keychain (accessible across your devices) and as a fallback in the local device Keychain.

### Audit Trail
- The App maintains an append-only, tamper-detected change history for flights, aircraft, settings, and related records. Each entry is linked with a cryptographic hash chain to detect unauthorised modification.
- The audit trail is stored locally (and in iCloud if sync is enabled). It is never transmitted to MachCrit.

### No MachCrit Logbook Servers
The developer does not operate servers that store your logbook, Pilot Wallet, backups, or invoices. There are no MachCrit user accounts. All data belongs to you and lives under your control (on your device and in cloud services you enable).

---

## 5. Data Sharing

We do not sell, rent, trade, or otherwise share your personal information with third parties for their own purposes. The only disclosures of your data are:

| Recipient | What is shared | When | Your control |
|---|---|---|---|
| **Apple (iCloud/CloudKit)** | App data you sync | If iCloud Sync is enabled | Toggle in system Settings / Data & Cloud |
| **Apple Maps** | Map region being viewed | When a map is displayed | Stop using map views; maps are not required to keep a manual logbook |
| **FlightRadar24** (via Cloudflare proxy) | Aircraft registration + time window or GPS bounding box | If ADS-B Enrichment is enabled (Pro) | Toggle in Settings > Enhancements |
| **Apple Calendar** | Scheduled flight details | If Calendar Sync is enabled | Toggle in Settings > Calendar & Scheduling |
| **Cloud storage providers** (iCloud Drive, Dropbox, OneDrive, Google Drive) | AES-encrypted backup blob | If Cloud Backup is configured | Configure in Settings > Data & Cloud |
| **Apple (StoreKit)** | Subscription purchase interaction | When purchasing or restoring Pro | Managed by Apple |
| **Apple Intelligence** (if used on a supported device) | The prompt or document context for a Smart Assist request | If Smart Assist is enabled and Apple Intelligence handles the request | Disable Smart Assist; manage Apple Intelligence in system Settings |
| **A recipient you choose** | An exported report, invoice, backup, or shared file | When you use Share / Export | You choose the file and the destination |

---

## 6. Analytics & Advertising

MachCrit Logbook contains **no third-party analytics SDKs** (such as Firebase Analytics, Mixpanel, or Amplitude), **no advertising SDKs**, and **no crash-reporting services** (such as Crashlytics or Sentry). The App does not track you across other apps or websites.

---

## 7. Your Rights & Choices

**Access your data:** All your data is visible within the App at all times. You may also export a full encrypted backup via **Settings > Data & Cloud**.

**Delete your data:** You may delete individual flights, aircraft, airports, credentials, or other records from within the App. Deleting the App removes all local data. To remove data from iCloud, visit icloud.com and manage the App's container, or disable iCloud sync before deleting the App.

**Withdraw permissions:** You may revoke location, microphone, speech recognition, calendar, camera, photos, and Face ID / Touch ID permissions at any time in system **Settings > Privacy & Security**. Revoking a permission disables the related feature but does not affect data already stored.

**Opt out of enrichment and assist:** Disable ADS-B Enrichment, schedule matching, and Smart Assist in **Settings > Enhancements**.

**Opt out of iCloud Sync:** Toggle off in system iCloud settings or **Settings > Data & Cloud**.

**Portability:** Your data can be exported as an encrypted backup, and selected records can be exported as reports, at any time from the App.

If you are in South Africa, the EEA, the United Kingdom, or another jurisdiction with data-protection rights, see Section 10.

---

## 8. Data Retention

The App retains your data for as long as you use it. There is no automatic expiry. If you delete the App, all local data is removed. iCloud data persists until you remove it manually via iCloud.com or by restoring from a backup that does not contain it.

The App's audit trail is append-only by design (it cannot be selectively deleted). This is a data integrity feature, not a retention policy imposed by the developer. You can clear the entire audit trail by importing a fresh backup that pre-dates the events you wish to remove.

---

## 9. Children's Privacy

MachCrit Logbook is a professional and personal aviation record-keeping tool. It is not directed at children under the age of 13, and we do not knowingly collect personal information from children under 13.

If you are in a jurisdiction that requires a higher age of consent for information-society services, the App is intended for users who can lawfully enter a contract and who hold, or are training toward, a pilot qualification. If you are a parent or guardian and believe a child has provided personal information through the App, please contact us so we can help you remove it.

---

## 10. International Users & South Africa (POPIA)

MachCrit Logbook is developed in South Africa and available globally via the Apple App Store.

**Responsible party:** Chad Clarke, reachable at chadclarke1@gmail.com.

Because logbook data is stored on your device (and, if you enable them, in Apple or other cloud services you choose), MachCrit does not operate a central personal-information database. Most access, correction, and deletion is done directly in the App.

### 10.1 South Africa — Protection of Personal Information Act (POPIA)

If you are in South Africa:
- The Developer is the responsible party only for personal information that actually reaches the Developer (for example an email you send, or a diagnostic export you attach). Logbook data that never leaves your device is processed on the device you control.
- You may request access to, correction of, or deletion of personal information the Developer holds, or object to processing, by emailing chadclarke1@gmail.com.
- You may lodge a complaint with the Information Regulator (South Africa).

### 10.2 EEA, United Kingdom, and similar regimes

- **Legal basis for processing:** Your data is processed on the basis of your consent (granting permissions and enabling optional features) and the performance of a contract (providing the logbook service you requested).
- **Your rights under GDPR / UK GDPR:** You have the right to access, rectify, erase, restrict processing of, and obtain a portable copy of your personal data, and to withdraw consent. To exercise these rights for data the Developer holds, contact chadclarke1@gmail.com. Since no logbook is stored on MachCrit servers, most of these rights are exercised directly within the App or through iCloud settings.
- **Data transfers:** If iCloud Sync, Apple Maps, Apple Intelligence, ADS-B Enrichment, or cloud backup is enabled, limited data is transferred to Apple, FlightRadar24 (via the proxy), or your chosen backup provider, which may be located outside your home jurisdiction. Those providers' terms and transfer mechanisms apply.

---

## 11. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will update the "Last Updated" date at the top of this page. Material changes will be noted in the App's release notes. Your continued use of the App after a change constitutes your acceptance of the revised policy.

The version history of this policy is available in the Git repository where it is maintained: [github.com/chadclarke1/machcrit-legal](https://github.com/chadclarke1/machcrit-legal).

---

## 12. Contact

If you have questions, concerns, or requests regarding this Privacy Policy or your data:

**Chad Clarke**  
Email: chadclarke1@gmail.com

---

*This policy covers MachCrit Logbook for iPhone, iPad, and Apple silicon Mac. It does not cover third-party services such as Apple iCloud, Apple Maps, Apple Intelligence, FlightRadar24, Dropbox, OneDrive, or Google Drive, each of which has its own privacy policy.*
