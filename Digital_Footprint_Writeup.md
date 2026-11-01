# TryHackMe CTF Writeup: Digital Footprint

**Platform:** TryHackMe  
**Challenge:** Digital Footprint  
**Category:** OSINT (Open-Source Intelligence)  
**Difficulty:** Not specified  
**Operating System:** Kali Linux  
**Author:** xplo01t-z3ro

---

## 1. Introduction

The Digital Footprint challenge focuses on Open-Source Intelligence (OSINT) techniques to investigate digital artifacts and extract useful information.

Throughout this challenge, I analyzed image metadata, investigated timestamps, identified geographical landmarks, and extracted hidden information from document metadata.

The main objective was to discover publicly available information and hidden clues that could help solve each task and retrieve the flags.

## 2. Tools Used

The following tools and techniques were used during the investigation:

- **ExifTool:** Extracting metadata from images and documents.
- **Google Maps:** Investigating geographical coordinates.
- **Google Search:** Identifying locations and landmarks.
- **Visual Analysis:** Examining image details and identifying recognizable locations.
- **Metadata Analysis:** Extracting timestamps, usernames, document properties, and other hidden information.

---

## 3. Task 1 – Identifying the Location Through Image Metadata

### Objective
Identify the geographical location associated with the provided image.

### Step 1: Download and Inspect the Image

First, I downloaded the provided image and examined its metadata using ExifTool.

Command:

```bash
exiftool edited-house-1763031553617.jpg
```

### Step 2: Analyze EXIF Metadata

The command returned several metadata fields, including:

```text
File Name       : edited-house-1763031553617.jpg
File Type       : JPEG
Image Width     : 1306
Image Height    : 837
GPS Latitude    : 26 deg 12' 14.76"
GPS Longitude   : 28 deg 2' 50.28"
GPS Position    : 26 deg 12' 14.76", 28 deg 2' 50.28"
```

The most important information was the GPS coordinates embedded in the image metadata.

### Step 3: Identify the Location

I used the extracted GPS coordinates to investigate the geographical location through mapping services.

The coordinates pointed to Johannesburg, South Africa.

**Flag:**

```text
THM{Johannesburg}
```

---

## 4. Task 2 – Timestamp Investigation

### Objective
Identify the required timestamp and retrieve the corresponding flag.

### Investigation

I examined the provided evidence and identified the timestamp required to answer the task.

The extracted timestamp was:

```text
20160210224602
```

**Flag:**

```text
THM{20160210224602}
```

> **Note:** The original notes contain the final timestamp and screenshots but do not preserve the exact extraction commands or intermediate investigation steps.

---

## 5. Task 3 – Landmark Identification

### Objective
Identify the location of the landmark shown in the provided image.

### Step 1: Visual Inspection

I examined the supplied landmark image and focused on recognizable architectural and geographical characteristics.

### Step 2: Location Investigation

Using the visual evidence and geographical research, I investigated the landmark and identified the location as the General Post Office.

### Result

The identified landmark was:

```text
General Post Office
```

**Flag:**

```text
THM{General Post Office}
```

---

## 6. Task 4 – Extracting Hidden Information from Document Metadata

### Objective
Investigate the metadata of the provided internal document and discover hidden information.

### Step 1: Inspect the Document

The provided file was an OpenDocument Text (ODT) document.

I used ExifTool to extract its metadata.

Command:

```bash
exiftool internal-docs-1769695301727.odt
```

### Step 2: Analyze Document Metadata

The output revealed several interesting metadata fields:

```text
File Name       : internal-docs-1769695301727.odt
File Type       : ODT
Creation-date   : 2026:01:29 14:59:44
Description     : Just remember Robin, don't publish this externally!
Subject         : Key Updates
Title           : Internal Document
Generator       : LibreOffice/25.8.4.2
Editing-cycles  : 4
Editing-duration: PT29M54S
```

### Step 3: Discover the Hidden Username

While reviewing the metadata, I found a particularly interesting user-defined field:

```text
User-defined Name : Internal username
User-defined      : markwilliams7243
```

This revealed the internal username stored in the document's metadata.

The username was an important clue for completing the investigation.

**Flag:**

```text
THM{Y0u_f0und_7h3_fin4l_fl4g!}
```

---

## 7. Final Flags

All four tasks were successfully completed.

| Task | Result | Flag |
|---|---|---|
| Task 1 | Johannesburg | `THM{Johannesburg}` |
| Task 2 | Timestamp | `THM{20160210224602}` |
| Task 3 | General Post Office | `THM{General Post Office}` |
| Task 4 | Final Flag | `THM{Y0u_f0und_7h3_fin4l_fl4g!}` |

---

## 8. Key Takeaways

This challenge provided practical experience with several important OSINT investigation techniques.

1. **Image Metadata Analysis:** Learned how to extract GPS coordinates and other information from image metadata using ExifTool.
2. **Timestamp Investigation:** Practiced identifying relevant timestamp information from digital evidence.
3. **Visual Geolocation:** Improved the ability to recognize landmarks and identify geographical locations.
4. **Document Metadata Analysis:** Learned how document properties can expose internal usernames and other potentially sensitive information.
5. **Digital Footprint Awareness:** Understood how publicly accessible digital artifacts can reveal information that users may not realize they are exposing.

## 9. Conclusion

The Digital Footprint challenge demonstrated how seemingly harmless digital files can contain valuable intelligence.

By analyzing image EXIF data, investigating timestamps, identifying landmarks, and examining document metadata, I successfully completed all four tasks.

This challenge strengthened my practical understanding of OSINT methodologies and highlighted the importance of metadata awareness in cybersecurity investigations.

**Challenge Status: Completed**
