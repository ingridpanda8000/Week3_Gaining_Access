# # Week 3: Gaining Access - PDF Password Cracking with Johnny and Networkwalks tools

## Cybersecurity Internship Assignment

### 📌 Overview
This week focuses on gaining access to password-protected PDF files using **Johnny** - the GUI frontend for John the Ripper on Windows and Network walks tools.

---

### 🎯 Objectives
- Extract password hashes from encrypted PDF files
- Use Johnny GUI to perform dictionary attacks
- Successfully crack passwords and access locked documents

---

### 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **Johnny** | GUI frontend for John the Ripper |
| **John the Ripper** | Password cracking engine |
| **pdf2john.exe** | Extract PDF password hashes |

---


---

### 🔧 Step-by-Step Process

#### Step 1: Install Johnny on Windows

1. Download John the Ripper from https://www.openwall.com/john/
2. Extract to `C:\john`
3. Download Johnny from https://github.com/openwall/johnny/releases
4. Install and launch Johnny
5. Go to **Settings** → Set John path to `C:\john\run\john.exe`

![Johnny Configuration](screenshots/johnny_config.png)

#### Step 2: Extract PDF Hash

Open Command Prompt as Administrator:

```cmd
cd C:\john\run
pdf2john.exe "C:\path\to\locked_document.pdf" > hash.txt
