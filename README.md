# 🔐 Password Auditing & PDF Hash Cracking — Week 3

A hands-on cybersecurity practical focused on **password auditing, PDF hash extraction, dictionary-based password attacks, and password security** using Kali Linux and John the Ripper.

---

## 🛡️ Disclaimer

All activities were performed in an **authorized cybersecurity training environment** for educational purposes.

Password auditing and cracking techniques should only be used on files, systems, or accounts that you own or have explicit permission to test.

---

## 🧰 Tools Used

| Tool | Purpose |
|---|---|
| `Kali Linux` | Cybersecurity testing environment |
| `pdf2john` | Extract password hash information from PDF files |
| `John the Ripper` | Password auditing and dictionary attacks |
| `rockyou.txt` | Password wordlist |
| `Linux Terminal` | Command-line operations |

---

## 🔎 1. PDF Hash Extraction

The first step was to extract the password hash information from the password-protected PDF files.

### 1.1 pdf2john

#### Command

pdf2john protected.pdf > hash.txt

#### Purpose

`pdf2john` was used to process the protected PDF and extract information that could be used by John the Ripper for password auditing.

#### Observation

- PDF password hash information was successfully extracted.
- The extracted output was saved for further analysis.

---

## 🔑 2. Password Auditing with John the Ripper

After extracting the hash, John the Ripper was used to perform a dictionary-based password audit.

### 2.1 Dictionary Attack

#### Command

john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt

#### Purpose

The command uses the `rockyou.txt` wordlist to test commonly used passwords against the extracted hash.

#### Observation

- John the Ripper successfully processed the hash.
- Password candidates from the wordlist were tested.
- The assigned lab challenge was successfully completed.

---

## 📋 3. Password Recovery Verification

After the password was recovered, the result was verified using John the Ripper.

#### Command

john --show hash.txt

#### Purpose

Used to display the recovered password information associated with the tested hash.

#### Result

The required passwords for the assigned challenge were successfully recovered in the authorized lab environment.

> For privacy and responsible disclosure, the actual passwords, hashes, and challenge flags are not published in this repository.

---

## 🧪 4. Lab Workflow

The overall process followed during the practical was:

Password-Protected PDF
        ↓
     pdf2john
        ↓
    Hash Output
        ↓
 John the Ripper
        ↓
  rockyou.txt
        ↓
 Password Recovery
        ↓
   Result Verification

---

## 📊 5. Key Findings

- Password-protected files can be subjected to offline password auditing.
- Weak or commonly used passwords are more susceptible to dictionary attacks.
- Wordlists can significantly improve password auditing efficiency.
- `pdf2john` can prepare supported PDF password information for John the Ripper.
- John the Ripper is useful for authorized password security testing.
- Strong, unique passwords are an important part of protecting sensitive files.

---

## 🧠 6. What I Learned

This practical strengthened my understanding of password security and offensive security techniques.

### Key Learning Areas

- 🔹 Password hash extraction
- 🔹 PDF password auditing
- 🔹 Dictionary-based attacks
- 🔹 John the Ripper
- 🔹 Linux command-line operations
- 🔹 Wordlist-based password testing
- 🔹 Password security
- 🔹 Responsible security testing
- 🔹 Secure documentation of cybersecurity labs

---

## 📸 7. Screenshots

### Screenshot 1 — PDF 1
![Hash Extraction](Hash%20Extraction.png)

### Screenshot 2 — PDF 2
![John the Ripper](John%20the%20Ripper.png)

### Screenshot 3 — PDF 3
![Password Recovery](pdf3%20cracked.png)

> Note: Update the image paths above to match your actual screenshot filenames in the `images/` folder.

---

## 📁 8. Repository Structure

Week-3-Password-Auditing-Lab/
│
├── README.md
├── Hash Extraction.png
├── John the Ripper.png
└── pdf3 cracked.png

---

## 🛡️ 9. Security & Privacy

To keep this repository safe for public viewing:

- Real passwords are not published.
- Password hashes are not published.
- Challenge flags are not published.
- Personal information is not included.
- Sensitive terminal output should be removed or masked before uploading screenshots.

This documentation focuses on the learning process and techniques rather than exposing challenge answers.

---

## 🎓 10. Conclusion

Week 3 provided hands-on experience with password auditing and PDF hash cracking in an authorized cybersecurity training environment.

Using `pdf2john`, John the Ripper, and the `rockyou.txt` wordlist, I practiced the workflow of extracting password hash information, performing dictionary-based auditing, and verifying results.

The practical reinforced the importance of strong passwords, secure access controls, responsible security testing, and careful handling of sensitive information.

---

## 👨‍💻 Author

**Muhammad Asad Sattar**  
BS Computer Science Student | Cybersecurity Intern | Cybersecurity Learner  

**Skills Practiced:**  
`Cybersecurity` `Password Auditing` `John the Ripper` `pdf2john` `Kali Linux` `Linux` `Ethical Hacking` `Password Security` `Cybersecurity Labs`

---

## ⚠️ Disclaimer

This project was completed for authorized educational and cybersecurity training purposes only. Do not use password auditing or cracking techniques against files, systems, or accounts without explicit authorization.
