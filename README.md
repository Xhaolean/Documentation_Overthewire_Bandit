🛡️ OverTheWire: Bandit — Complete Walkthrough & Documentation

Welcome to my OverTheWire: Bandit cybersecurity learning repository.

This repository documents my hands-on progress through the Bandit wargame, including the commands I used, the reasoning behind each solution, Linux concepts learned, mistakes encountered, and important security concepts.

The goal is not simply to collect passwords, but to build a practical understanding of Linux, command-line tools, networking, authentication, file permissions, automation, and basic security concepts.

---

📌 About OverTheWire Bandit

Bandit is a beginner-oriented Linux wargame hosted by OverTheWire. Each level presents a security-related challenge that requires investigation and problem-solving from the command line.

Key Learning Areas

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

📊 Progress & Learning Log

Level| Focus Concept| Writeup| Status
00 → 01| SSH Connection & Basic Credentials| "Level 00 → 01" (Levels/Level00_01.md)| ✅ Completed
01 → 02| Handling Special Filenames| "Level 01 → 02" (Levels/Level01_02.md)| ✅ Completed
02 → 03| Spaces in Filenames & Quoting| "Level 02 → 03" (Levels/Level02_03.md)| ✅ Completed
03 → 04| Hidden Files & Dotfiles| "Level 03 → 04" (Levels/Level03_04.md)| ✅ Completed
04 → 05| File Identification with "file"| "Level 04 → 05" (Levels/Level04_05.md)| ✅ Completed
05 → 06| Searching by File Attributes| "Level 05 → 06" (Levels/Level05_06.md)| ✅ Completed
06 → 07| System-wide Search & Permissions| "Level 06 → 07" (Levels/Level06_07.md)| ✅ Completed
07 → 08| Text Filtering with "grep"| "Level 07 → 08" (Levels/Level07_08.md)| ✅ Completed
08 → 09| Sorting & Unique Lines| "Level 08 → 09" (Levels/Level08_09.md)| ✅ Completed
09 → 10| Extracting Strings| "Level 09 → 10" (Levels/Level09_10.md)| ✅ Completed
10 → 11| Base64 Decoding| "Level 10 → 11" (Levels/Level10_11.md)| ✅ Completed
11 → 12| ROT13 / Caesar Cipher| "Level 11 → 12" (Levels/Level11_12.md)| 🔄 In Progress
12 → 13| Hex Dump & Decompression| —| ⏳ Upcoming
13 → 14| SSH Private Key Authentication| —| ⏳ Upcoming
14 → 15| Local Network Services| —| ⏳ Upcoming
15 → 16| TLS Connections| —| ⏳ Upcoming
16 → 17| Port Scanning & RSA Keys| —| ⏳ Upcoming
17 → 18| File Comparison & "diff"| —| ⏳ Upcoming
18 → 19| Shell Escaping| —| ⏳ Upcoming
19 → 20| SUID Binaries| —| ⏳ Upcoming
20 → 21| Network Sockets & SUID| —| ⏳ Upcoming
21 → 22| Cron Jobs| —| ⏳ Upcoming
22 → 23| Shell Script Analysis| —| ⏳ Upcoming
23 → 24| Scheduled Script Injection| —| ⏳ Upcoming
24 → 25| PIN Brute Force| —| ⏳ Upcoming
25 → 26| Restricted Shell Escape| —| ⏳ Upcoming
26 → 27| SUID & Shell Escape| —| ⏳ Upcoming
27 → 28| Git Repository Inspection| —| ⏳ Upcoming
28 → 29| Git History & Credentials| —| ⏳ Upcoming
29 → 30| Git Branches & Hidden Commits| —| ⏳ Upcoming
30 → 31| Git Tags| —| ⏳ Upcoming
31 → 32| Git Push & Hooks| —| ⏳ Upcoming
32 → 33| Restricted Shell Escape| —| ⏳ Upcoming
33 → 34| Final Level| —| ⏳ Upcoming

«Note: The progress table will be updated as I complete each level and publish its documentation.»

---

🧪 Documentation Methodology

For each level, I document:

1. Objective — What the challenge is asking.
2. Initial Investigation — What I inspected before attempting a solution.
3. Commands Used — Relevant Linux commands and syntax.
4. Reasoning — Why each command was used.
5. Solution — How the challenge was solved.
6. Concept Learned — The underlying Linux/security concept.
7. Mistakes & Lessons — Problems encountered and how I corrected them.

The focus is on understanding the methodology rather than simply recording the final answer.

---

💻 Environment Setup

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

🧠 What I Am Learning

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

These concepts form part of my broader cybersecurity learning journey.

---

📈 Progress

Current Level: 11 → 12

Levels Completed: 11

Levels Remaining: 23

Primary Tools Learned So Far:

Linux CLI
grep
sort
uniq
strings
file
find
cut
tr
base64
xxd
SSH

---

⚠️ Responsible Use

All techniques documented here are performed within the intentionally vulnerable OverTheWire Bandit environment.

The purpose of this repository is educational: to document my learning, improve my Linux and cybersecurity skills, and demonstrate my problem-solving process.

These techniques should only be applied to systems where I have explicit authorization to test.

---

📚 Resources

- OverTheWire: https://overthewire.org/
- Bandit: https://overthewire.org/wargames/bandit/

---

👤 About This Repository

This is a personal cybersecurity learning project.

Rather than only documenting whether I completed a challenge, I am using the repository as a technical record of what I investigated, why I made certain decisions, what went wrong, and what I learned from the process.

The documentation will continue to evolve as I progress through the remaining Bandit levels.