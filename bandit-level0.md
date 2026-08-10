# Bandit Level 0
- **Date:** 2026-07-10
- **Target:** Connecting to bandit.labs.overthewire.org (over Port 2220) using SSH

---

### 1. Objective

to establish a connection to `bandit.labs.overthewire.org` over `Port 2220` using Secure Shell (SSH)

### 2. Commands used

`ssh`: command used to establish connection with a server using username and ip address and can be used with `-p` flag to explicitly use another port other than `Port 22`

### 3. Syntax

`ssh bandit[*]@bandit.labs.overthewire.org -p 2220`

### 4. Steps:

- the process is quite simple. Using the aforementioned command with proper username we send a request to establish a connection.
- once the connection and authenticity of the host is established, the server prompts up the password
- once entered and processed the connection is established.
