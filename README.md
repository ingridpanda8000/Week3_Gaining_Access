# Week 3: Gaining Access - Password Cracking with Johnny and Networkwalks Tools.

## Cybersecurity Internship Assignment

### 📌 Overview
This week focuses on gaining access to password-protected PDF files using two tools:
1. **Johnny** - GUI frontend for John the Ripper
2. **Networkwalks Tools** - Hash Calculator & Password Cracker

### 💡 Key Learnings
- Hash extraction from PDFs
- Dictionary attacks with Johnny
- Cracking with Networkwalks tools
- Password security importance
---

## Using Johnny.
### 🎯 Objectives
- Extract password hashes from encrypted PDF files using online tool
- Use Johnny GUI to perform dictionary attacks
- Successfully crack passwords and access locked documents

---

### 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **Johnny** | GUI frontend for John the Ripper |
| **John the Ripper** | Password cracking engine |
| **Online PDF Hash Extractor** | Extract PDF password hashes |

---

## 🔧 Step-by-Step Process

### Step 1: Install Johnny
1. Download from: https://github.com/openwall/johnny/releases
2. Install and launch
3. Go to **Settings** → Set path: `JTR_John CLI Win x64\john-1.9.0-jumbo-1-win64\run`

![Johnny Config](Screenshots_week3/adding_johnny_Cl.png)

### Step 2: Extract PDF Hash
1. Go to: https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php
2. Upload PDF → Click **Upload**
3. Copy the hash

![Extract Hash](Screenshots_week3/online_hash_extractor.png)

### Step 3: Save Hash
1. Open Notepad
2. Paste hash
3. Save as `pdf_1.txt` in `hashes/` folder

![Save Hash](Screenshots_week3/online_hash_extractor.png)

### Step 4: Load Hash in Johnny
1. Open Johnny
2. Click **File** → **Open Password File**
3. Select `pdf_1.txt`

![Load Hash](Screenshots_week3/saved_hashes.png)


### Step 5: Start Cracking
1. Click **Start Attack** button
2. Johnny begins cracking
3. Progress shown in status bar:
   - Speed (passwords/sec)
   - Time elapsed
   - Passwords attempted

![Cracked Password](Screenshots_week3/cracked_password.png)

---

## 📊 Results

| PDF File | Cracked Password |
|----------|------------------|
| My Locked PDF1 | good-luck |
| My Locked PDF2 | password1 |
| My Locked PDF3 | good-luck |

---

# Password Cracking with Networkwalks tools

### 📌 Overview
Using Networkwalks tools to crack password-protected PDF files. The process involves two steps:
1. **Hash Calculator** - Extract hash from PDF
2. **Password Cracker** - Crack the extracted hash using wordlists

---

### 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **Networkwalks Hash Calculator** | Extract PDF password hashes |
| **Networkwalks Password Cracker** | Crack hashes using wordlists |

---
### Steps
1. Open Hash Calculator → Upload PDF → Get Hash
![Hash calculator](Screenshots_week3/Hash_calculator.png)

3. Copy hash
5. Open Password Cracker → Load hash
   ![Password_craker](Screenshots_week3/password_cracking.png)
7. Select wordlist (built-in or custom)
8. Click Start → View cracked password

### Results
| PDF File | Cracked Password |
|----------|------------------|
| My Locked PDF1 | good-luck |
| My Locked PDF2 | password1 |
| My Locked PDF3 | good-luck |

### 📸 Proof of Access
![pdf1](Screenshots_week3/pdf1_networkwalks.png)
![pdf2](Screenshots_week3/pdf2_networkwalks.png)
![pdf3](Screenshots_week3/pdf3_networkwalks.png)

![pdf1](Screenshots_week3/pdf1.png)
![pdf2](Screenshots_week3/file_2.png)
![pdf3](Screenshots_week3/pdf3.png)
