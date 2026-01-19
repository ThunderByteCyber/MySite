
# TryHackMe Lab: Digital Forensics Case B4DM755

## Overview

This write‑up documents my approach to a simulated digital forensics and incident response (DFIR) investigation based on the TryHackMe – Digital Forensics Case: B4DM755 lab. The purpose of this post is to demonstrate forensic methodology, tool usage, and investigative reasoning in a portfolio‑safe manner, without disclosing sensitive answers, flags, or step‑by‑step solutions.

The scenario focuses on a corporate espionage investigation involving the suspected theft of trade secrets. I acted as the first responder and forensic analyst responsible for evidence handling, forensic imaging, and initial analysis.

This lab made extensive use of FTK Imager, a tool I am already familiar with through my Cyber Forensics studies at Murdoch University, including previous forensic assignments and practical labs.

In a real-world investigation, a write-blocking device would be used when mounting forensic artefacts to prevent accidental modification of evidence. This principle was reinforced during the lab.

---

## Investigation Objectives

The key objectives of the investigation were:

1. Apply legally defensible digital forensics procedures
2. Preserve and document evidence using chain of custody principles
3. Create a forensically sound image of seized media
4. Perform high‑level analysis of files and metadata
5. Interpret findings in the context of a criminal investigation

---

## Forensic Methodology

The investigation followed standard DFIR phases commonly used in law‑enforcement and corporate investigations:

1. **Preparation & Legal Authority** – Understanding the scope of the investigation and ensuring legal authority (search and seizure considerations)
2. **Identification & Preservation** – Locating digital evidence and preventing contamination or alteration
3. **Collection** – Acquiring evidence using forensic tools and write‑blocking techniques
4. **Examination & Analysis** – Reviewing file systems, metadata, and artefacts
5. **Reporting** – Documenting findings in a clear, defensible manner

This structured approach ensures that evidence remains admissible and defensible if presented in legal proceedings.

---

## Evidence Handling and Acquisition

During the simulated search, removable media was identified as potential evidence. Proper evidence handling procedures were applied, including:

- Documenting the evidence prior to examination
- Using write‑blocking to prevent modification
- Maintaining continuity through chain of custody documentation

**Tools Used:**

- FTK Imager – for evidence identification, preview, and forensic imaging
- A full forensic image of the media was created using a raw (dd) format with hash verification enabled to ensure integrity

---

## Forensic Imaging Process

Key forensic acquisition steps included:

1. Verifying the media was not encrypted prior to imaging
2. Selecting an appropriate image format for compatibility and integrity
3. Generating cryptographic hashes to confirm image authenticity
4. Verifying that the forensic image matched the source media

This process ensures that all analysis is conducted on a verified copy rather than the original evidence.

---

## High‑Level Analysis Approach

After acquisition, analysis focused on file system structure and artefact review, including:

- Reviewing file listings and directory structures
- Identifying deleted or hidden files
- Examining file metadata for indicators such as:
  * Creation and modification timestamps
  * File type mismatches
  * Embedded metadata (e.g., EXIF data)

---

## Investigative Reasoning

Throughout the investigation, artefacts were interpreted within the broader case context. Examples of reasoning applied include:

1. Correlating timestamps to reconstruct potential activity timelines
2. Assessing whether file concealment techniques were used
3. Identifying how metadata may link a suspect to locations or events
4. Recognising indicators of deliberate data handling or exfiltration

---

## Key Skills Demonstrated

This lab allowed me to demonstrate and strengthen the following skills:

- Digital evidence handling and preservation
- Forensic imaging and verification
- Use of industry‑standard tools (FTK Imager)
- Metadata analysis and interpretation using FTK Imager and ExifTool
- Investigative documentation and reporting
- Legal and ethical awareness in digital forensics

---

## Reflection

This exercise reinforced the importance of process over answers in digital forensics. Proper documentation, integrity verification, and structured reasoning are critical for producing reliable and defensible findings.

The lab also highlighted how small artefacts, such as metadata or file inconsistencies, can provide valuable investigative leads when analysed in context.

Rather than focusing on challenge answers, the analysis emphasised how evidence can reveal user behaviour, timelines, and intent — a core skill in digital forensics.

This analytical process mirrors real‑world DFIR investigations where technical findings must support investigative hypotheses.

---

## Acknowledgement

I would like to acknowledge the Digital Forensics Case B4DM755 lab provided by TryHackMe as the foundation for the practical components of this write-up. This interactive room simulates a realistic digital forensics investigation where the learner assumes the role of a DFIR First Responder and Forensics Lab Analyst tasked with acquiring and analysing digital evidence for use in a hypothetical court case.

The lab incorporates key forensic principles — including the preservation of the chain of custody, the use of FTK Imager for forensic disk imaging, and evidence analysis — through a structured scenario involving a fictitious suspect charged with corporate espionage and theft of trade secrets. The scenarios and guided tasks within this lab have directly informed the procedures and discussions presented in this report.

[Link to TryHackMe Lab](https://tryhackme.com/room/caseb4dm755)



