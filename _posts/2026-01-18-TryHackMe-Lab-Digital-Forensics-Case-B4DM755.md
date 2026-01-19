# TryHackMe Lab: Digital Forensics Case B4DM755

<br>

#### <ins> The Lab </ins>


1. Overview

This write‑up documents my approach to a simulated digital forensics and incident response (DFIR) investigation based on the TryHackMe – Digital Forensics Case: B4DM755 lab. The purpose of this post is to demonstrate forensic methodology, tool usage, and investigative reasoning in a portfolio‑safe manner, without disclosing sensitive answers, flags, or step‑by‑step solutions.

The scenario focuses on a corporate espionage investigation involving the suspected theft of trade secrets. I acted as the first responder and forensic analyst responsible for evidence handling, forensic imaging, and initial analysis.

<br>

2. Investigation Objectives

The key objectives of the investigation were:
<ol>

<li>Apply legally defensible digital forensics procedures</li>

<li>Preserve and document evidence using chain of custody principles</li>

<li>Create a forensically sound image of seized media</li>

<li>Perform high‑level analysis of files and metadata</li>

<li>Interpret findings in the context of a criminal investigation</li>

</ol>

<br>

3. Forensic Methodology

The investigation followed standard DFIR phases commonly used in law‑enforcement and corporate investigations:
<ol>

<li>Preparation & Legal Authority – Understanding the scope of the investigation and ensuring legal authority (search and seizure considerations)</li>

<li>Identification & Preservation – Locating digital evidence and preventing contamination or alteration</li>

<li>Collection – Acquiring evidence using forensic tools and write‑blocking techniques</li>

<li>Examination & Analysis – Reviewing file systems, metadata, and artefacts</li>

<li>Reporting – Documenting findings in a clear, defensible manner</li>

<li>This structured approach ensures that evidence remains admissible and defensible if presented in legal proceedings.</li>
</ol>

<br>

4. Evidence Handling and Acquisition

During the simulated search, removable media was identified as potential evidence. Proper evidence handling procedures were applied, including:
<ol>

<li>Documenting the evidence prior to examination</li>

<li>Using write‑blocking to prevent modification</li>

<li>Maintaining continuity through chain of custody documentation</li>

Tool Used

<li>FTK Imager – for evidence identification, preview, and forensic imaging</li>

<li>A full forensic image of the media was created using a raw (dd) format with hash verification enabled to ensure integrity.</li>
</ol>

<br>

5. Forensic Imaging Process

Key forensic acquisition steps included:

<ol>

</li>Verifying the media was not encrypted prior to imaging</li>

<li>Selecting an appropriate image format for compatibility and integrity</li>

<li>Generating cryptographic hashes to confirm image authenticity</li>

<li>Verifying that the forensic image matched the source media</li>

<li>This process ensures that all analysis is conducted on a verified copy rather than the original evidence.</li>
</ol>

<br>

6. High‑Level Analysis Approach

After acquisition, analysis focused on file system structure and artefact review, including:
<ol>

<li>Reviewing file listings and directory structures</li>

<li>Identifying deleted or hidden files</li>

<li>Examining file metadata for indicators such as:

<li>Creation and modification timestamps</li>

<li>File type mismatches</li>

<li>Embedded metadata (e.g., EXIF data)</li>

</ol>
Rather than focusing on challenge answers, the analysis emphasised how evidence can reveal user behaviour, timelines, and intent — a core skill in digital forensics.

<br>

7. Investigative Reasoning

Throughout the investigation, artefacts were interpreted within the broader case context. Examples of reasoning applied include:

<ol>

<li>Correlating timestamps to reconstruct potential activity timelines</li>

<li>Assessing whether file concealment techniques were used</li>

<li>Identifying how metadata may link a suspect to locations or events</li>

<li>Recognising indicators of deliberate data handling or exfiltration</li>

</ol>

This analytical process mirrors real‑world DFIR investigations where technical findings must support investigative hypotheses.

<br>

8. Key Skills Demonstrated

This lab allowed me to demonstrate and strengthen the following skills:
<ol>

<li>Digital evidence handling and preservation</li>

<li>Forensic imaging and verification</li>

<li>Use of industry‑standard tools (FTK Imager)</li>

<li>Metadata analysis and interpretation using FTK Imager and exiftool</li>

<li>Investigative documentation and reporting</li>

<li>Legal and ethical awareness in digital forensics</li>
</ol>

<br>

9. Reflection

This exercise reinforced the importance of process over answers in digital forensics. Proper documentation, integrity verification, and structured reasoning are critical for producing reliable and defensible findings.

The lab also highlighted how small artefacts, such as metadata or file inconsistencies, can provide valuable investigative leads when analysed in context.

<br>

10. Acknowledgement

I would like to acknowledge the Digital Forensics Case B4DM755 lab provided by TryHackMe as the foundation for the practical components of this write-up. This interactive room simulates a realistic digital forensics investigation where the learner assumes the role of a DFIR First Responder and Forensics Lab Analyst tasked with acquiring and analysing digital evidence for use in a hypothetical court case. The lab incorporates key forensic principles — including the preservation of the chain of custody, the use of FTK Imager for forensic disk imaging, and evidence analysis — through a structured scenario involving a fictitious suspect charged with corporate espionage and theft of trade secrets. The scenarios and guided tasks within this lab have directly informed the procedures and discussions presented in this report. 
[Link to TryHackMe Lab](https://tryhackme.com/room/caseb4dm755)  







