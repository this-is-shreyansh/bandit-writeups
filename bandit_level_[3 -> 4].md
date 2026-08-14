# Bandit Level[3] -> Level[4]

-**Date:**  15-08-2026
-**Target:** hidden file in `inhere` directory

---

### 1. Objective: 

to access the hidden file in the `inhere` directory and access the password for the next level

### 2. Commands used
`ls`
`cd`
`cat`

### 3. Methodology

- using the password obtained from previous level along with the username `bandit3@bandit` we connect to the server over the port 2220
- once the connection is established we run the `ls` command to find the `inhere` directory.
- using the `cd` command we access the `inhere` directory
- using the `ls` command yields no result as all the files in the directory are hidden, thus, we use it along with `-a` flag to view all the hidden files present in the directory
- using the command reveals a file `...Hiding-From-You`
- using the `cat` command we read the password stored in the file.

### 4. Syntax

`ssh bandit3@bandit.labs.overthewire.org -p 2220`
`ls`
`cd inhere`
`ls -a`
`cat ...Hiding-From-You`

### 5. Takeaway

using the `-a` flag along with `ls` command to find out the hidden files in a directory

### 6. Retrieved Credentials
<!-- Store the key/password found for the next level. -->
- **Level [Next] Password:** `[REDACKTED_OR_PASSWORD]`
