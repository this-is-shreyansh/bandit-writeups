# Bandit Level[2] -> Level[3]

-**Date:** 15-08-2026

-**Target:** `-- spaces in this filename--`

---

### 1. Objective

Obtaining the password stored in a file called `-- spaces in this filename--` located in the home directory

### 2. Commands used

`ls`
`cat`

  ### 3. Methodology

- using the password obtained in the last level and the username `bandit2` we establish a ssh connection over the port 2220.
- once established we use the `ls` command to check the files present in the home directory.
- we find the `--spaces in this filename--` present in the home directory.
- using the `cat` command we access the content of the file and thus the password.

### Syntax

`ls`
`cat -- '--spaces in this filename--'`

### 4. Takeaway:

In accessing files or directories that contain whitespaces between their name, we need to put their entire name within quotation marks (`''`) to access them.

### 5. Retrieved Credentials
<!-- Store the key/password found for the next level. -->
- **Level [3] Password:** `[REDACKTED_PASSWORD]`
