# Digital_forensics Lab

A hands-on didgital forensics project covering disk imaging, file system analysis, browser forensics, anti-forensics techniques, and live system capture. Each section documents real investigative workflows using industry-standard tools on actual evidence media.

# About

This repository documents a practical digital frensics lab built to simulate real-world evidence acquisition and analysis workflows. The focus is on maintainig forensic integrity through out the investigation process, by creating bit-for-bit imaging of the usb drive, capturing the memory, analyzing memory dumps, browser forensics and viewing anti-forensics technqies.

| Tool | Purpose |
| --- | --- |
| dcfldd | Forensic disk imaging with hash verification |
| Autopsy | GUI-based file system analysis and deleted file recovery |
| FTK Imager | Forensic image acuisition and evidence preview |
| Browser artefacts toosl | Viewing browsers data such as history, cookies and cached data |
| volatitlty | command line tool to analyse data in memory |
| shred | command line tool used to  delete files, or overwrite them to make it unrecoverable even by the forensics tools |

# Topics Covered 

# 1. Disk Imaging with dcfldd:

dcfldd is a forensics tool used to create bit-for-bit image of a drive while generating a hash log to verify and protect the integerity of the acquired image.

Notes: After acquiring the disk image; the best practice is to always store the original and create another copy for
analysis to prevent any contamination of the evidence.

see  [`dcfldd.md`](dcfldd.md) for walkthrough

# 2. Evidence analysis with autopsy

Autopsy is used to anayse the forensic image of the USB drive. The lab demonstrates how to load an image file, browse the full file system, identify file types, and recover deleted files for further analysis.

see 

# 3. FTK Imager
FTK Imager is used for forensic image acquisition and initial evidence preview. It provides a fast way to verify image integrity and preview file content without altering the original evidence.

# 4. Browser Forensics

Covers the extraction and analysis of browser artefacts including browsing history, download records, cookies and cached files. These artefacts can reveal user activity and timelines critical to an investigation.

# 5. Linux forensics

Forensic analysis techniques appilied to linux systems, including file system examination, log analysis, and artefact recovery.

# 6. Live system capture (windows and linux)

Documents the process of ccapturing a live windows and linux system's volatitle data - including running processes, network connections, memory - before powering down where the data would be lost.

Notes: When the system is live, the decryption key is loaded in the RAM or memory.

# 7. Anti-forensics

Covers techniques used to hide, alter or destroy evidence that are used in the wild.


# Disclaimer
This lab is built entirely for educational purposes in an isolated, controlled environment. All techniques demonstrated here are performed on systems and media owned and controlled by the author. Performing forensic or offensive techniques on systems without explicit authorisation is illegal and unethical.
