# Bandit Level 0 — First SSH Connection

## Objective

The objective of Level 0 is to connect to the OverTheWire Bandit server using SSH.

The challenge provides:

* **Username:** `bandit0`
* **Password:** `bandit0`
* **Host:** `bandit.labs.overthewire.org`
* **Port:** `2220`

The main concept introduced in this level is **SSH (Secure Shell)** and how to connect to a remote Linux machine from the command line.

---

## Initial Investigation

Before connecting, understand how SSH works and what information is required to establish a connection.

An SSH connection generally needs:

```text
username + hostname/IP + port
```

The standard SSH syntax can be checked from the Linux manual:

```
man ssh
```

The general syntax is:

```
ssh [options] [user@]hostname
```

The Bandit server uses port `2220` instead of the usual SSH port `22`, so the port needs to be specified manually.

---

## Commands Used

### 1. Open the terminal

On a Linux desktop, the terminal can commonly be opened with:

```
Ctrl + Alt + T
```

The terminal provides a command-line interface (CLI), which allows commands to be executed directly.

---

### 2. Checking SSH manual

```
man ssh
```

This displays the manual page for the SSH client.

---

### 3. Connect to the Bandit server

```
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

Breaking the command down:

```
ssh
│
└── Program used to establish an SSH connection

bandit0@
│
└── Username of the remote account

bandit.labs.overthewire.org
│
└── Hostname of the remote machine

-p 2220
│
└── Connect using port 2220
```

When prompted for the password enter:

```
bandit0
```

---

## Initial File Investigation
See what files were available in the current directory.
```
ls
```

`ls` lists the contents of the current directory.

```
ls -a
```
can be used to include hidden files and directories in the listing.

---

## Additional Investigation

### System information

```bash
uname -a
```

This displays information about the system, including the Linux kernel and system architecture.

### Network information

```bash
hostname -I
```

This displays the IP addresses associated with the host.

These commands were not required to solve the level, use them to understand the environment.

---

## Reasoning

```text
Access a remote Linux machine
        ↓
SSH is designed for remote shell access
        ↓
Requirement:  username + host + port
        ↓
The challenge provides all three
        ↓
The server uses port 2220 instead of the default 22
        ↓
Use ssh with the -p option
        ↓
Authenticate with the provided password
```

---

## Solution

The essential command was:

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

Password:

```text
bandit0
```

After authentication, the SSH session connected to the `bandit0` account on the Bandit server.

---

## Concept Learned

### 1. SSH

SSH (Secure Shell) is a protocol used to securely access and interact with a remote computer.

Instead of running commands on my own computer:

```text
My Computer → Local Shell
```

SSH allows you to obtain a shell on another machine:

```text
My Computer
     │
     │ SSH
     ▼
Remote Linux Server
     │
     ▼
Remote Shell
```

Commands entered after logging in are executed on the remote machine.

### 2. Ports

A network service listens for connections on a particular port.

SSH commonly uses:

```text
22
```

The Bandit server uses:

```text
2220
```

Therefore, explicitly specify it with:

```bash
-p 2220
```

### 3. Remote hostname

Instead of directly entering an IP address, connect using:

```text
bandit.labs.overthewire.org
```

This is a hostname that identifies the remote server.

---

## Final Takeaway

Bandit Level 0 introduced me to the basic workflow of interacting with a remote Linux machine:

```text
Find connection details
        ↓
Understand SSH syntax
        ↓
Connect to remote server
        ↓
Authenticate
        ↓
Inspect the remote environment
```

The main concepts were **SSH, remote shells, usernames, hostnames, ports, authentication, and basic Linux environment inspection**.
