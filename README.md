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

1. Disk Imaging with dcfldd
dcfldd is a forensics tool used to create bit-for-bit image of a drive while generating a hash log to verify and protect the integerity of the acquired image.

Notes: After acquiring the disk image; the best practice is to always store the original and create another copy for
analysis to prevent any contamination of the evidence.



Lets start the project
