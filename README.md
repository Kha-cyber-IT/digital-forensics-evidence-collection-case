# Digital Forensics Investigation: Residential Burglary

**Case Number:** 2025-03847  
**Investigation Type:** Digital Evidence Identification and Preservation  
**Environment:** NetDevGroup DF-101 Forensic-WS / Ubuntu Linux  
**Case Date:** 16 March 2025  
**Project Type:** Practical Digital Forensics Case Study (Simulation)

> **Disclaimer:** This is a simulated investigation completed for educational and portfolio purposes. The evidence records, device details, and custody transfers are training materials, not records of an actual criminal investigation. No real devices were seized or imaged.

---

## 1. Case Background

A homeowner reported a residential burglary in which approximately **$15,000 worth of electronics and jewellery** had been stolen overnight.

Responding patrol officers secured the property. The home office contained several electronic devices that could potentially establish:

- When the burglary occurred.
- Whether digital devices recorded suspicious activity.
- Whether relevant communications or transactions occurred.
- Whether devices contain files, logs, or other investigative leads.

The investigation focused on identifying digital evidence, assessing volatility, documenting device conditions, selecting preservation methods, and maintaining chain-of-custody records.

## 2. Investigation Objectives

1. Identify all potential digital evidence sources.
2. Document their locations, power states and physical conditions.
3. Prioritise evidence according to the order of volatility.
4. Review simulated crime-scene photographs.
5. Determine suitable evidence preservation procedures.
6. Prepare evidence identification and device documentation records.
7. Create a simulated chain-of-custody log.
8. Record custody transfers and evidence integrity considerations.

## 3. Digital Evidence Identified

| Evidence ID | Device | Location | Power State | Collection Priority |
|---|---|---|---|---|
| E-001 | Desktop computer | Home office desk | Powered on | 1 - Immediate |
| E-002 | Smartphone | Desk beside keyboard | On, screen locked | 2 - Urgent |
| E-003 | Tablet | Couch in adjacent sitting area | Powered off | 3 - Standard |
| E-004 | Amazon Echo smart speaker | Bookshelf | Powered on | 2 - Urgent |
| E-005 | USB flash drive | Top desk drawer | Not connected | 3 - Standard |

### Evidence E-001: Desktop Computer

**Observation:** The desktop was powered on, displaying a spreadsheet containing financial information, including account numbers and transaction amounts.

**Risk:** Volatile memory could contain running processes, open files, network connections and encryption keys.

**Preservation decision:**
- Photograph the active display before interaction.
- Keep the computer powered on.
- Request a forensic examiner to perform live acquisition.
- Preserve RAM and obtain a forensic disk image using approved procedures.

**Priority:** 1 - Immediate.

### Evidence E-002: Smartphone

**Observation:** The smartphone was on the desk next to the keyboard. Its screen was locked, with message and email notification banners visible.

**Network indicators:** Wi-Fi and Bluetooth were recorded in the lab scenario.

**Preservation decision:**
- Photograph the lock screen, time and notifications.
- Protect the device from remote network access.
- Use an appropriate Faraday enclosure under forensic handling procedures.
- Avoid unnecessary interaction with the device.

**Priority:** 2 - Urgent.

### Evidence E-003: Tablet

**Observation:** A powered-off tablet with a cracked screen was found on the couch in the adjacent sitting area.

**Preservation decision:**
- Keep the tablet powered off.
- Document the existing screen damage.
- Package it in padded anti-static protection.
- Apply an evidence label and tamper-evident seal.

**Priority:** 3 - Standard.

### Evidence E-004: Amazon Echo

**Observation:** An Amazon Echo smart speaker was powered on on a bookshelf, with an active blue ring indicator.

**Preservation decision:**
- Photograph the device and illuminated indicator.
- Preserve its current state pending forensic guidance.
- Record the model and account information only if visible.
- Consider preservation of relevant cloud records through appropriate legal procedures.

**Priority:** 2 - Urgent.

### Evidence E-005: USB Flash Drive

**Observation:** A USB flash drive was located in the top desk drawer, partially hidden beneath papers. The simulated scene photograph showed a SanDisk Ultra 64GB device labelled "Backup 2024".

**Preservation decision:**
- Photograph the drive in its original location.
- Avoid connecting it to an ordinary computer.
- Package it in a suitable protective evidence envelope.
- Seal, label and document the item.
- Arrange forensic imaging and hashing during laboratory examination.

**Priority:** 3 - Standard.

---

## 4. Order of Volatility

Evidence was prioritised according to the likelihood that information could be lost or altered.

| Priority | Evidence | Main Concern |
|---|---|---|
| 1 - Immediate | Desktop | Loss of volatile RAM data |
| 2 - Urgent | Smartphone | Remote wiping and changing notifications |
| 2 - Urgent | Amazon Echo | Changing device state and cloud-record retention |
| 3 - Standard | Tablet | Stable powered-off storage |
| 3 - Standard | USB drive | Stable nonvolatile storage |

The desktop was prioritised because volatile memory can be permanently lost when power is interrupted.

## 5. Crime Scene Photography

Five simulated scene photographs were used to document device locations and observable conditions.

| Photograph | Evidence Covered | Documentation Purpose |
|---|---|---|
| `scene_overview.jpg` | E-001 to E-005 | Overall scene layout and evidence locations |
| `desk_closeup.jpg` | E-001, E-002, E-005 | Desktop screen, smartphone and desk area |
| `couch_tablet.jpg` | E-003 | Tablet location and cracked screen |
| `bookshelf_echo.jpg` | E-004 | Smart speaker position and blue ring indicator |
| `drawer_usb.jpg` | E-005 | USB drive location, markings and surrounding papers |

### Scene Photographs

The original simulated photographs can be placed in the `scene-photos/` directory.

The README links below will display them once those files are added.

**Scene overview**

![Home office overview](scene-photos/scene_overview.jpg)

**Desktop and smartphone**

![Desktop and smartphone close-up](scene-photos/desk_closeup.jpg)

**Tablet**

![Tablet with cracked screen](scene-photos/couch_tablet.jpg)

**Amazon Echo**

![Amazon Echo on bookshelf](scene-photos/bookshelf_echo.jpg)

**USB flash drive**

![USB flash drive in desk drawer](scene-photos/drawer_usb.jpg)

---

## 6. Chain of Custody

A simulated chain-of-custody register was prepared for all five evidence items.

Each entry documents:

- Evidence identification number and description.
- Collection date and location.
- Device condition.
- Serial-number visibility.
- Collector identity.
- Initial forensic hash status.
- Evidence transfers and their purposes.

The original scene date was **2025-03-16**.

Where serial numbers were not recorded, the documentation uses:

`Not visible without manipulation`

Where forensic imaging had not yet occurred, the relevant initial hash status is:

`N/A, to be computed upon forensic imaging`

### Simulated Custody Transfers — E-001

| Transfer | Released By | Received By | Purpose |
|---|---|---|---|
| 1 | learner (First Responder) | FE-Smith (Forensic Examiner) | RAM acquisition and forensic disk imaging |
| 2 | FE-Smith (Forensic Examiner) | EC-Johnson (Evidence Custodian) | Secure evidence locker storage |

The exercise schedules Transfer 1 thirty minutes after collection and Transfer 2 two hours after Transfer 1.

**These are simulated handoffs, not verified historical custody events.**

---

## 7. Tools and Environment

| Tool / Environment | Purpose |
|---|---|
| Ubuntu Linux | Case documentation environment |
| NetDevGroup Forensic-WS | Hosted digital forensics training laboratory |
| Konsole | Linux terminal operations |
| Python 3 | Automated creation and updating of documentation |
| Kate | Reviewing and editing evidence forms |
| Gwenview | Reviewing simulated scene photographs |
| Git / GitHub | Version control and portfolio publication |

### Python Automation

Python was used to create and organise the case documentation, including:

- Evidence identification records.
- Device state and preservation documentation.
- Photograph registers.
- Simulated chain-of-custody records.
- CSV evidence register.

The Python scripts automate documentation, not forensic acquisition or analysis.

## 8. Project Structure

```text
Case-2025-03847/
├── README.md
├── README.txt
├── records/
│   ├── 00-CASE-OVERVIEW.txt
│   ├── 01-EVIDENCE-IDENTIFICATION.txt
│   ├── 02-DEVICE-DOCUMENTATION.txt
│   ├── 03-PHOTOGRAPH-REGISTER.txt
│   ├── 04-CHAIN-OF-CUSTODY.txt
│   ├── 05-EVIDENCE-REGISTER.csv
│   └── 06-FORENSIC-WORKFLOW.txt
└── scene-photos/
    ├── scene_overview.jpg
    ├── desk_closeup.jpg
    ├── couch_tablet.jpg
    ├── bookshelf_echo.jpg
    └── drawer_usb.jpg
```

Photographs appear in the project only after the original simulated JPG files are added.

## 9. Skills Demonstrated

- Digital evidence identification.
- Crime scene documentation.
- Order-of-volatility assessment.
- Device preservation planning.
- Network isolation considerations.
- Digital evidence photography.
- Chain-of-custody documentation.
- Evidence integrity and forensic hashing concepts.
- Linux command-line operations.
- Python documentation automation.
- Git-based case organisation.

## 10. Limitations and Next Steps

This project covers **initial digital evidence identification, documentation and preservation planning**.

The following activities were not performed or independently verified:

- Live RAM acquisition.
- Forensic disk imaging.
- Cryptographic hash computation for the five devices.
- Deleted-file recovery.
- File-system or timeline analysis.
- Actual evidence collection or custody transfer.

The recreated case documents were based on the lab instructions and available screenshots rather than an exported copy of the complete original scene report. Unverified details should be checked before updating the records.

Future practical work may include forensic imaging, hash verification, Autopsy analysis and evidence timeline reconstruction using authorised training datasets.

---

## Conclusion

This simulated residential burglary investigation demonstrates the importance of documenting digital evidence before handling devices, preserving volatile information, choosing appropriate preservation methods and maintaining an accountable chain of custody.

The exercise provides practical experience in the initial stages of digital forensic investigations while establishing a foundation for more advanced acquisition and analysis labs.

**Case:** 2025-03847  
**Category:** Digital Forensics / Evidence Collection and Preservation  
**Status:** Educational simulation
