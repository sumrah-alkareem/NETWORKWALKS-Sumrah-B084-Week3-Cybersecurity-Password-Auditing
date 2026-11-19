# NETWORKWALKS-Sumrah-B084-Week3-Cybersecurity-Password-Auditing

**Week 3 Internship Tasks – PDF Password Recovery and Hash Analysis (W3-PM1 & W3-PM2)**

---

## Overview

As part of Week 3 of the Networkwalks Cybersecurity Internship, I worked on practical exercises involving password security, PDF hash extraction, and password recovery techniques.

The tasks involved examining encrypted PDF documents, extracting their password hashes, and testing their resistance to dictionary-based attacks using two different approaches: a locally installed password auditing application and Networkwalks' browser-based tools.

This week's work was divided into two practical modules:

- **W3-PM1:** Offline PDF Password Recovery using John the Ripper (Johnny GUI).
- **W3-PM2:** PDF Hash Extraction and Password Auditing using Networkwalks Online Tools.

---

## Tools and Technologies

| Tool | Application |
|---|---|
| Windows 11 | Operating environment for local testing |
| John the Ripper (Johnny) | GUI-based password auditing |
| PDF Hash Extraction Tool | Extracts password hashes from encrypted PDFs |
| Networkwalks Hash Calculator | Browser-based PDF hash extraction |
| Networkwalks Password Cracker | Dictionary-based password testing |

---

## Practical Tasks

### 1. W3-PM1 – Offline PDF Password Auditing with Johnny

**Objective:** Examine three password-protected PDF documents by extracting their cryptographic hashes and testing them with John the Ripper to recover their passwords.

**Work Completed:**

1. Prepared Johnny and configured it to work with John the Ripper on Windows.
2. Processed three encrypted PDF documents through a hash extraction utility.
3. Saved the extracted hash data into separate text files.
4. Imported the hash files into Johnny and initiated dictionary-based password auditing.
5. Successfully recovered the passwords for all three documents.
6. Opened the PDFs using the recovered passwords and verified the embedded flags.

**Results – W3-PM1**

| PDF Document | Hash File | Recovered Password | Result |
|---|---|---|---|
| My Locked PDF1.pdf | hash1.txt | `good-luck` | Successfully verified |
| My Locked PDF2.pdf | hash2.txt | `password1` | Successfully verified |
| My Locked PDF3.pdf | hash3.txt | `1qaz2wsx` | Successfully verified |

**Evidence and Screenshots**

- `pdf1.png` – Johnny configuration and setup.
- `pdf2.png` – Password recovery result.
- `flag1.jpg` – Verification flag from the first PDF.
- `flag2.jpg` – Verification flag from the second PDF.

---

### 2. W3-PM2 – PDF Password Auditing with Networkwalks Tools

**Objective:** Use Networkwalks' online utilities to extract and audit the password hash of another encrypted PDF document, followed by cross-verification of the previous exercise.

**Work Completed:**

1. Accessed the Networkwalks Hash Calculator and PDF Hash Extractor.
2. Uploaded the designated encrypted PDF document to obtain its password hash.
3. Submitted the extracted hash to the Networkwalks Password Cracker.
4. Performed a dictionary-based password audit using the available wordlist.
5. Successfully identified the password as `password1`.
6. Opened the protected PDF and verified its embedded flag.
7. Compared the earlier PDF recovery results with the Networkwalks platform.

**Evidence and Screenshots**

- `hashcalculator.jpg` – Networkwalks Hash Calculator interface.
- `pdfhashextractor.jpg` – PDF hash extraction process.
- `passwordcracking.jpg` – Dictionary attack and recovered password.
- `flag1pm2.jpg` – Final verification flag.

---

## Consolidated Results

| Module | Target | Recovered Password | Verification |
|---|---|---|---|
| W3-PM1 | PDF 1 | `good-luck` | Successful |
| W3-PM1 | PDF 2 | `password1` | Successful |
| W3-PM1 | PDF 3 | `1qaz2wsx` | Successful |
| W3-PM2 | PDF 1 (NW Lab) | `password1` | Successful |

**Overall Result:** All four PDF password recovery exercises were completed successfully, and the corresponding verification flags were obtained.

---

## What I Learned

- **Password Predictability:** Common passwords and keyboard-based patterns can be identified through dictionary attacks.
- **Hash Extraction:** Learned how password verification data can be extracted from encrypted PDF documents.
- **Offline Password Auditing:** Gained practical experience using John the Ripper to examine extracted hashes.
- **Different Auditing Approaches:** Compared locally installed tools with browser-based password auditing utilities.
- **Importance of Strong Passwords:** Understood why long, unique, and unpredictable passphrases are essential for protecting sensitive documents.

### Security Recommendations

- Avoid common words, predictable sequences, and keyboard patterns.
- Use long and unique passphrases for sensitive documents.
- Never reuse passwords across different accounts or files.
- Protect password hashes from unauthorized access.
- Use modern password hashing schemes such as Argon2id, bcrypt, or yescrypt where appropriate for stored credentials.

---

## Ethical Considerations

All activities documented in this repository were performed as part of authorized educational exercises using sample PDF documents supplied for the Networkwalks internship.

The purpose of these exercises was to understand password security weaknesses and learn how to assess them responsibly. Password auditing and recovery should only be performed on files and systems for which proper authorization has been granted.

---

## Acknowledgment

Special thanks to **Networkwalks Academy** and my mentor **Waqas Karim (CCIE)** for providing practical cybersecurity exercises that helped me develop a better understanding of password auditing and cryptographic hash analysis.

---

## Author

**Sumrah Al kareem**

Cybersecurity & Digital Forensics Student

**Program:** Networkwalks Cybersecurity Internship  
**Batch:** B084  
**Week:** 03
