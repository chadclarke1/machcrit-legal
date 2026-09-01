# Privacy Policy — MachCrit Logbook

**Last Updated:** September 1, 2026  
**Effective Date:** September 1, 2026  
**Applies to:** MachCrit for iPhone, iPad, and Apple silicon Mac (App Store version 1.95 and later)

---

MachCrit Logbook ("the App", "we", "our") is developed and maintained by **Chad Clarke** ("the Developer") as an independent Apple application. This Privacy Policy explains what information the App collects, how it is used and protected, when (if ever) it leaves your device, and what choices you have as a user.

Please read this policy carefully. By using the App you acknowledge that you have read and understood it.

**Contact:** chadclarke1@gmail.com

**Summary of this update:** This policy reflects the current App, including Pilot Wallet, Smart Assist, document-assisted import, App Lock, airport records, reports, Family Sharing, **Mapbox Maps SDK as a MachCrit Pro feature**, Mapbox telemetry disclosure and opt-out, and availability **worldwide except the Russian Federation and the People's Republic of China**. The on-device, no-account model is unchanged. The Developer does not guarantee accuracy, retention, or regulatory compliance of any data in the App.

---

## 1. Overview

MachCrit is a personal convenience logbook. It is designed to operate primarily on-device. It has no MachCrit user accounts, no registration process, and no MachCrit servers that store your logbook.

All data you enter is stored locally on your device and, if you choose, optionally synced to your own iCloud account or backed up to a cloud storage provider of your choice.

The Developer-operated network components are limited to:
- an optional ADS-B enrichment proxy (see Section 3); and
- Mapbox map traffic that occurs when you use MachCrit Pro maps (see Section 2.12).

Neither is a MachCrit logbook database. The proxy does not create accounts. Mapbox is a third-party mapping provider.

The App does not sell, rent, or trade your personal information to any third party.

**Availability.** MachCrit is offered through the Apple App Store in territories where Apple makes it available. It is **not offered in the Russian Federation or the People's Republic of China**. Availability can change.

**No guarantee.** The Developer does not guarantee the accuracy, completeness, retention, backup, availability, or regulatory compliance of any information in or produced by the App. Remaining lawful is your responsibility. See the Terms of Use.

---

## 2. Information We Collect

### 2.1 Location Data

**What is collected:**
When you start a flight recording, the App uses your device's GPS to capture continuous location data: latitude, longitude, altitude, speed, heading, and timestamp. These points form your flight track. Outside of active recording, the App may use low-power significant-location monitoring to detect when a potential flight begins.

**Why it is collected:**
- To record flight tracks for your logbook
- To auto-detect takeoff and landing times
- To calculate duration, distance, average speed, and maximum altitude
- To display your track on a map
- To enrich completed flights with ADS-B data (Pro, opt-in — see Section 3)
- When MachCrit Pro maps are in use, location and map-viewport data may also be sent to Mapbox as described in Section 2.12

**Where it is stored:**
Track points are stored in an encrypted local database on your device. If iCloud Sync is enabled, track points are included in the data synced to your iCloud account (encrypted end-to-end by Apple).

**Permissions required:**
- "Always" location access (for background flight detection and continuous track capture)
- Precise location access (requested when you first record)

You can revoke location permissions at any time in **iOS / iPadOS / macOS Settings > Privacy & Security > Location Services > MachCrit**. Revoking location access will disable flight auto-detection, track recording, and map features that need location. Manual logbook entry continues to work.

Granting location permission is your affirmative consent for the App to access location for the purposes above. It is separate from Mapbox Telemetry, which you can opt out of as described in Section 2.12.

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
To display currency status, pre-fill logbook fields, personalise the App, and keep a convenient on-device record of licences and medicals.

**Where it is stored:**
Locally on your device in an encrypted database. If iCloud Sync is enabled, this data is synced to your iCloud account. This information is never transmitted to MachCrit for the Developer's own purposes.

Pilot Wallet is a personal convenience display. It is **not** an official digital licence, medical certificate, or credential issued by any aviation authority. The Developer does not verify, certify, or guarantee any credential you store.

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
To maintain your personal pilot logbook, support currency tracking for supported rule sets, generate reports, and (if you use them) invoices.

**Where it is stored:**
Locally on your device. Optionally synced to iCloud. Never transmitted to MachCrit servers.

The Developer does not audit, certify, or guarantee these records.

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
To associate flights with departure and arrival locations, support search and reporting, and keep a personal airport list.

**Where it is stored:**
In a local database on your device, together with a bundled or updated reference airport dataset. User-added airports and notes are optionally synced to iCloud.

The reference dataset is for convenience only. It is not an aeronautical chart, AIP, or operational airport directory. It may be incomplete, outdated, or wrong.

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
Locally on your device. Optionally synced to iCloud and/or Apple Calendar (see Section 2.11).

You are responsible for having a lawful basis to store other people's names and details.

---

### 2.7 Voice Dictation (Microphone)

**What is collected:**
If you use voice dictation to enter flight remarks, the App captures audio from your device's microphone solely for transcription. Transcription is performed **on your device** using Apple's Speech Recognition framework. No audio is recorded, stored, or transmitted by MachCrit.

**What is stored:**
Only the resulting plain text. No audio file is retained.

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

The App may use on-device Vision, Optical Character Recognition, and (where available) Apple Intelligence / Foundation Models to propose structured fields from that material.

**Why it is collected:**
To reduce manual data entry. Proposed values are suggestions only until you review and save them. They may be wrong.

**Where it is stored:**
Extracted text and the resulting logbook records are stored locally (and in iCloud if sync is enabled). Original images or files are stored only if you keep them attached to a record. Imported content is not uploaded to MachCrit servers.

**Permissions that may be requested when you use these features:**
- Camera
- Photo Library
- Files / document picker access

These permissions are optional. Declining them disables import-from-camera or import-from-photos; manual entry continues to work.

**What is NOT done:**
MachCrit does not send your documents to a developer-operated AI service, and does not use imported documents to train models for other users.

---

### 2.9 Smart Assist (Pro Feature — Opt-In)

**What it is:**
Smart Assist is an optional Pro feature that can provide on-device assistance such as suggested field values, smart import help, flight-intelligence summaries, and related suggestions. It is **off by default** and can be turned off in **Settings > Enhancements**.

**What data is processed:**
Only the logbook, document, or field context needed for the suggestion you requested.

**Where processing happens:**
Assistance is intended to run **on your device** using Apple system frameworks. On supported devices with Apple Intelligence enabled, Apple's on-device Foundation Models may be used. If Apple routes a request through Apple Intelligence Private Cloud Compute, that processing is performed by Apple under [Apple's Privacy Policy](https://www.apple.com/privacy/), not on MachCrit servers.

**What we never see:**
The Developer does not receive your prompts, documents, or Smart Assist outputs.

Smart Assist suggestions are convenience aids. They are not certified aviation data, legal advice, or a substitute for your own verification.

---

### 2.10 Client Information & Invoicing

**What is collected:**
If you use invoicing and billing features, you may enter:
- Company name, contact name, email address, phone number, and mailing address
- Invoice amounts, flight references, and related billing notes

**Why it is collected:**
To generate flight invoices on your device.

**Where it is stored:**
Locally on your device. Optionally synced to iCloud. Never transmitted to MachCrit servers. If you export or share an invoice, the recipient sees whatever you chose to send.

You are responsible for tax, invoicing, and privacy law that applies to those records.

---

### 2.11 Calendar Data

**What is collected:**
If you enable Calendar Sync in Settings, the App reads and writes events to your Apple Calendar. Events may contain scheduled flight details: callsign, departure and arrival airports, crew names, aircraft tail number, and notes.

**Why it is collected:**
To provide bidirectional scheduling between MachCrit and your system calendar.

**Where it is stored:**
In your Apple Calendar on-device. If your device uses iCloud Calendar, Apple handles that sync.

**Permissions required:**
Calendar access. Calendar sync is **off by default** and can be disabled in **Settings > Calendar & Scheduling**.

---

### 2.12 Maps — Apple Maps and Mapbox (MachCrit Pro)

Maps in MachCrit are for reviewing recorded tracks and locating airports in your logbook. They are **not** certified charts and are **not** for navigation, flight planning, or in-flight operational use.

#### Apple Maps / MapKit

Where Apple Maps is used, map display may cause your device to request map tiles from Apple. Apple may receive the map region being viewed. That processing is governed by [Apple's Privacy Policy](https://www.apple.com/privacy/).

#### Mapbox Maps SDK (MachCrit Pro)

MachCrit Pro uses the **Mapbox Maps SDK for iOS** (Mapbox, Inc.) to display maps. This is a paid-product feature. If you do not subscribe to Pro, Mapbox map traffic from this SDK is not used for that Pro map experience.

**What may leave your device when you use Pro maps:**

| Data | Why Mapbox receives it |
|---|---|
| Map viewport (the geographic area and zoom level you view) | To return map tiles and styles |
| IP address | To deliver the service, billing, and security. Mapbox states it deletes IP addresses after 30 days unless needed for an investigation |
| Device, SDK, and randomly generated billing / session identifiers | To operate and bill the Maps SDK |
| Location and usage telemetry (de-identified location, altitude, accuracy, session ID) | Mapbox Telemetry, used by Mapbox to improve maps. Sent by default when the SDK gathers location unless you opt out |

**What is NOT sent to Mapbox by MachCrit:**
Pilot name, licence or certificate numbers, hours, remarks, crew names, medical status, Pilot Wallet contents, invoices, or your Core Data logbook store.

Mapbox processes this data as an independent controller / service operator under the [Mapbox Privacy Policy](https://www.mapbox.com/legal/privacy). Mapbox's location platform is hosted in the cloud (including the United States). Your use of Pro maps is also subject to the [Mapbox Terms of Service](https://www.mapbox.com/legal/tos).

**Telemetry opt-out (required disclosure):**
Mapbox's terms require that you can opt out of Mapbox Telemetry. In MachCrit this is provided through the **Mapbox attribution control** on the map (the information / (i) control). If that control is visible, use it to turn Mapbox Telemetry off. You can also revoke Location Services for MachCrit in system Settings, which stops the App (and the SDK) from accessing GPS.

Opting out of telemetry does not delete map tiles already requested. Maps may still send viewport and IP data needed to render tiles.

The Developer does not operate Mapbox, does not control Mapbox's retention, and does not guarantee Mapbox availability or map accuracy.

---

### 2.13 Reports, Exports & Sharing

You may generate reports and export records (for example PDF, CSV, or encrypted backup) and share them through the system share sheet, AirDrop, Mail, Files, or another app you choose.

**What leaves your device:**
Only the file you explicitly export or share, and only to the destination you select. MachCrit does not upload exports to a MachCrit server.

You are responsible for choosing recipients, for remaining lawful in what you share, and for redacting information you do not wish to disclose.

---

### 2.14 App Lock & Biometrics

If you enable App Lock, the App uses the device passcode, Face ID, or Touch ID through Apple's Local Authentication framework.

**What is collected:**
Only a local setting that App Lock is enabled. The App does not receive, store, or transmit your biometric templates. Face ID and Touch ID data remain in the Secure Enclave.

App Lock is a convenience. It is not a guarantee against data loss, device theft, backup exposure, or iCloud access on another device you have signed in.

---

### 2.15 Subscription Status

**What is collected:**
The App checks whether you hold an active Pro subscription via Apple's StoreKit 2 framework. The App stores only a local entitlement state.

**What we never see:**
Your Apple ID, payment method, billing address, or full payment receipts. Billing is handled entirely by Apple.

**Subscription products:**
- MachCrit Pro Monthly (`com.cwr.MachCrit.pro.monthly`)
- MachCrit Pro Annual (`com.cwr.MachCrit.pro.annual`)

If Family Sharing is enabled on your Apple ID, a Pro subscription may be shared with your Family Sharing group according to Apple's rules. The Developer does not manage Family Sharing.

---

### 2.16 Device Identifier

**What is collected:**
A randomly generated device identifier (UUID) is created the first time you install the App on a device and stored in the device Keychain. It persists across app reinstalls on the same hardware.

**Why it is collected:**
Solely for sync conflict resolution when the same data is edited on multiple devices.

**Where it is stored:**
In the device Keychain. It is never transmitted to MachCrit servers. It is included in iCloud sync metadata only to the extent CloudKit uses it internally.

This identifier is separate from Mapbox's billing / session IDs described in Section 2.12.

---

### 2.17 On-Device Diagnostics

**Settings > Advanced Features** may include developer diagnostics and troubleshooting tools. Diagnostic logs are generated on your device.

Diagnostics are not sent automatically. They are not processed by Crashlytics, Sentry, or any other third-party crash service. If you contact support, you may optionally attach a diagnostic export; only then would the Developer see the content you chose to send.

---

## 3. ADS-B Enrichment (Pro Feature — Opt-In)

MachCrit Pro may attempt to match your completed flight against public ADS-B data provided by FlightRadar24 (FR24). This can fill departure and arrival airports, callsigns, or supplemental track points.

This data **may be incomplete, delayed, or incorrect**. The Developer does not guarantee it.

**What data leaves your device when this feature is active:**

| Data sent | Purpose |
|---|---|
| Aircraft registration (tail number) | Match your flight against FR24 ADS-B records |
| Flight time window (takeoff ± 5 minutes, landing ± 5 minutes) | Narrow the search |
| GPS bounding box (min/max lat/lon ± ~6 NM) | Used only if no aircraft is selected |

**What is NOT sent:**
Pilot name, licence numbers, hours, remarks, crew names, medical status, Pilot Wallet contents, imported documents, invoices, or other personal information.

**How the request is routed:**
Queries go through a Cloudflare Worker proxy operated by the Developer, then to FlightRadar24's REST API. The proxy does not store your logbook and is not intended to log query content. FlightRadar24's privacy policy governs their handling of the incoming request (aircraft registration, time window, and the proxy IP address).

**This feature is:**
- Disabled by default
- Requires a Pro subscription
- Can be turned off in **Settings > Enhancements**

---

## 4. Data Storage, Security & No Retention Guarantee

### On-Device Storage
- The Core Data database is protected with **NSFileProtectionComplete** (or the platform equivalent) while the device is locked.
- Automatic backups created by the App are encrypted with **AES-256-GCM** before being written to disk. The key is stored in the device Keychain.
- Optional App Lock adds a local gate using the system passcode or biometrics.

These measures reduce risk. They are **not** a warranty that your data cannot be lost, corrupted, accessed on an unlocked or backed-up device, or destroyed.

### iCloud Sync
- If enabled, your data is synced via Apple's CloudKit service. Apple encrypts this data end-to-end. The Developer has no access to your iCloud data and **does not control** whether Apple retains, syncs, or deletes it.
- You can disable iCloud sync in system Settings under iCloud, or from **Settings > Data & Cloud** where that control is provided.

### Cloud Backups (Optional)
- You may store encrypted backups in iCloud Drive, Dropbox, OneDrive, or Google Drive.
- Backups are encrypted with AES-256-GCM **before** they leave your device.
- The encryption passphrase is stored in iCloud Keychain and as a fallback in the local Keychain.
- Those providers' availability and retention are outside the Developer's control.

### Audit Trail
- The App maintains an append-only, tamper-detected change history for selected records. This is a local integrity aid, not a certified audit, not a legal hold, and not a retention guarantee.

### No MachCrit logbook servers
The Developer does not operate servers that store your logbook, Pilot Wallet, backups, or invoices. There are no MachCrit user accounts.

### No retention guarantee
The Developer **does not guarantee** that any data will be retained for any period. In particular:
- Deleting the App removes local data.
- Device loss, OS upgrade, restore, iCloud quota, a failed backup, a forgotten passphrase, or a provider outage can destroy or lock data.
- iCloud and third-party backups persist only according to those providers' rules, which the Developer does not control.
- There is no MachCrit-operated archive, disaster-recovery copy, or SLA.
- **You** are solely responsible for keeping whatever official, paper, or independent electronic records your regulator, employer, insurer, or examiner requires.

---

## 5. Data Sharing

We do not sell, rent, trade, or otherwise share your personal information with third parties for their own marketing. The only disclosures are:

| Recipient | What is shared | When | Your control |
|---|---|---|---|
| **Apple (iCloud/CloudKit)** | App data you sync | If iCloud Sync is enabled | Toggle in system Settings / Data & Cloud |
| **Apple Maps** | Map region being viewed | When an Apple map is displayed | Stop using that map view |
| **Mapbox** | Viewport, IP address, SDK/billing/session IDs, and (unless opted out) location telemetry | When you use MachCrit Pro maps | Do not use Pro maps; opt out of telemetry via the Mapbox (i) control; revoke Location Services |
| **FlightRadar24** (via Cloudflare proxy) | Aircraft registration + time window or GPS bounding box | If ADS-B Enrichment is enabled (Pro) | Toggle in Settings > Enhancements |
| **Apple Calendar** | Scheduled flight details | If Calendar Sync is enabled | Toggle in Settings > Calendar & Scheduling |
| **Cloud storage providers** | AES-encrypted backup blob | If Cloud Backup is configured | Configure in Settings > Data & Cloud |
| **Apple (StoreKit)** | Subscription purchase interaction | When purchasing or restoring Pro | Managed by Apple |
| **Apple Intelligence** | Prompt or document context for a Smart Assist request | If Smart Assist is enabled and Apple Intelligence handles it | Disable Smart Assist |
| **A recipient you choose** | An exported report, invoice, backup, or shared file | When you use Share / Export | You choose the file and destination |

The Developer may also disclose information if required by law, a court, or a competent authority, or to protect the Developer's legal rights — but only to the extent the Developer actually holds that information (typically an email or diagnostic you sent).

---

## 6. Analytics & Advertising

MachCrit itself contains **no third-party analytics SDKs** (such as Firebase Analytics, Mixpanel, or Amplitude), **no advertising SDKs**, and **no crash-reporting services** (such as Crashlytics or Sentry). The App does not track you across other apps or websites for advertising.

**Exception — Mapbox Telemetry:** the Mapbox Maps SDK used in MachCrit Pro includes Mapbox Telemetry as described in Section 2.12. That is Mapbox's location analytics for improving maps, not MachCrit advertising. You can opt out via the Mapbox attribution control.

---

## 7. Your Rights & Choices

**Access your data:** All your logbook data is visible in the App. You may export an encrypted backup via **Settings > Data & Cloud**.

**Delete your data:** You may delete individual records in the App. Deleting the App removes local data. To remove iCloud data, use icloud.com or disable iCloud sync before deleting the App.

**Withdraw permissions:** Revoke location, microphone, speech, calendar, camera, photos, and Face ID / Touch ID in system **Settings > Privacy & Security**.

**Opt out of enrichment and assist:** Disable ADS-B Enrichment, schedule matching, and Smart Assist in **Settings > Enhancements**.

**Opt out of Mapbox Telemetry:** Use the Mapbox attribution / (i) control on the map.

**Opt out of iCloud Sync:** System iCloud settings or **Settings > Data & Cloud**.

**Portability:** Export an encrypted backup or reports from the App. The Developer cannot retrieve a copy of your logbook from MachCrit servers because none exists.

If you are in South Africa, the EEA, the United Kingdom, or another jurisdiction with data-protection rights, see Section 10.

---

## 8. Data Retention

The App retains data on your device for as long as you keep it there. There is **no automatic MachCrit retention schedule** and **no promise** that data will still be there tomorrow.

If you delete the App, local data is removed. iCloud and cloud-backup copies persist until **you** remove them.

The audit trail is append-only by design. That is a local integrity feature, not a retention obligation on the Developer.

---

## 9. Children's Privacy

MachCrit is a personal aviation record-keeping tool. It is not directed at children under 13, and we do not knowingly collect personal information from children under 13.

The App is intended for users who can lawfully enter a contract and who hold, or are training toward, a pilot qualification. If you are a parent or guardian and believe a child has provided personal information through the App, contact us.

---

## 10. Territory, International Users & South Africa (POPIA)

**Responsible party:** Chad Clarke, South Africa, chadclarke1@gmail.com.

MachCrit is developed in South Africa and distributed on the Apple App Store **except in the Russian Federation and the People's Republic of China**. Do not use the App to circumvent that restriction.

Because logbook data is stored on your device (and, if you enable them, in Apple, Mapbox, FlightRadar24, or other services you choose), MachCrit does not operate a central personal-information database. Most access, correction, and deletion is done in the App.

### 10.1 South Africa — Protection of Personal Information Act (POPIA)

If you are in South Africa:
- The Developer is the responsible party only for personal information that actually reaches the Developer (for example an email you send, or a diagnostic export you attach). Logbook data that never leaves your device is processed on the device you control.
- You may request access to, correction of, or deletion of personal information the Developer holds, or object to processing, by emailing chadclarke1@gmail.com.
- You may lodge a complaint with the Information Regulator (South Africa).

### 10.2 EEA, United Kingdom, and similar regimes

- **Legal basis:** consent (permissions and optional features) and performance of a contract (providing the logbook tool you requested).
- **Your rights:** access, rectification, erasure, restriction, portability, and withdrawal of consent, to the extent they apply to data the Developer actually holds. Exercise logbook rights in the App; email chadclarke1@gmail.com for data the Developer holds.
- **Transfers:** If you enable iCloud, Apple Maps, Apple Intelligence, Mapbox Pro maps, ADS-B Enrichment, or cloud backup, limited data goes to those providers, which may process it outside your country (including the United States for Mapbox). Their terms apply. The Developer does not operate those transfers beyond offering the optional feature.

---

## 11. Changes to This Policy

We may update this Privacy Policy at any time. The "Last Updated" date will change. Material changes will be noted in the App's release notes where reasonably practicable. Continued use after publication is acceptance of the revised policy.

Version history: [github.com/chadclarke1/machcrit-legal](https://github.com/chadclarke1/machcrit-legal).

---

## 12. Contact

**Chad Clarke**  
Email: chadclarke1@gmail.com

---

*This policy covers MachCrit Logbook for iPhone, iPad, and Apple silicon Mac, as offered outside the Russian Federation and the People's Republic of China. It does not replace the privacy policies of Apple, Mapbox, FlightRadar24, Dropbox, OneDrive, Google Drive, or any other third party.*
