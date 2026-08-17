# OverTheWire: Bandit — Complete Walkthrough & Documentation

Welcome to my OverTheWire: Bandit cybersecurity learning repository.

This repository documents my hands-on progress through the Bandit wargame, including the commands I used, the reasoning behind each solution, Linux concepts learned, mistakes encountered, and important security concepts.

The goal is to build a practical understanding of Linux, command-line tools, networking, authentication, file permissions, automation, and basic security concepts.

---

# About OverTheWire Bandit

Bandit is a beginner-oriented Linux wargame hosted by OverTheWire. Each level presents a security-related challenge that requires investigation and problem-solving from the command line.

## Key Learning Areas

- 🐧 Linux CLI & Navigation
  
  - "ls", "cd", "pwd", "cat", "cp", "mv", "rm"
  - Hidden files and directory structures
  - File permissions and ownership

- 🔎 Text Processing & Analysis
  
  - "grep"
  - "sort"
  - "uniq"
  - "strings"
  - "cut"
  - "tr"
  - "file"
  - "xxd"

- 📦 Compression & Archives
  
  - "gzip"
  - "bzip2"
  - "tar"
  - Hexadecimal dumps
  - Nested compression

- 🌐 Networking
  
  - TCP connections
  - Port scanning
  - "nc" / Netcat
  - "openssl"
  - SSH
  - Network services

- 🔐 Authentication & Cryptography
  
  - SSH authentication
  - Private keys
  - Base64
  - ROT13 / Caesar cipher
  - TLS connections

- ⚙️ Linux Security
  
  - SUID binaries
  - SGID
  - Privilege boundaries
  - Cron jobs
  - Restricted shells
  - Shell escaping

- 📜 Git & Version Control Security
  
  - Git repositories
  - Commit history
  - Branches
  - Tags
  - Hidden credentials
  - Git hooks

---

📂 Repository Structure

Bandit/
│
├── README.md
│
└── Levels/
    ├── Level00_01.md
    ├── Level01_02.md
    ├── Level02_03.md
    ├── Level03_04.md
    ├── Level04_05.md
    ├── Level05_06.md
    ├── Level06_07.md
    ├── Level07_08.md
    ├── Level08_09.md
    ├── Level09_10.md
    ├── Level10_11.md
    ├── Level11_12.md
    ├── Level12_13.md
    ├── ...
    └── Level33_34.md

---

# 🧪 Documentation Format
1. Objective — What the challenge is asking.
2. Commands Used — Relevant Linux commands and syntax.
3. Reasoning — Why each command was used.
4. Solution — How the challenge was solved.
5. Concept Learned — The underlying Linux/security concept.
6. Mistakes & Lessons

---

# 💻 Environment Setup

The Bandit server can be accessed through SSH.

ssh banditX@bandit.labs.overthewire.org -p 2220

Replace "X" with the appropriate Bandit level.

Example:

ssh bandit11@bandit.labs.overthewire.org -p 2220

Useful Commands

pwd
ls
ls -la
cd
cat
file
find
grep
sort
uniq
strings
cut
tr
xxd
base64
ssh
The exact commands used will vary depending on the challenge.

---

# 🧠 Currently Learning

This repository is helping me build practical foundations in:

- Linux system administration
- Command-line investigation
- File systems
- File permissions
- Authentication
- Networking fundamentals
- Cryptography basics
- Shell scripting
- Process automation
- Git security
- Security-oriented problem solving

---

# ⚠️ Responsible Use

All techniques documented here are performed within the intentionally vulnerable OverTheWire Bandit environment.
These techniques should only be applied to systems where we have explicit authorization to test.
---

# 📚 Resources

- OverTheWire: https://overthewire.org/
- Bandit: https://overthewire.org/wargames/bandit/

---

# 👤 About This Repository
This repo will be a technical record of what I investigated and what went wrong, and what I learned from the process.
