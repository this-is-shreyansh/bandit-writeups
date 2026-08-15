# Bandit Level[4] -> Level [5]

- **Date:** 15-08-2026
- **Target:** human-readable file in the `inhere` directory

- ---

### 1. Objective:

accessing password for the next level stored in the only human-readable file in the `inhere` directory.

### 2. Commands used:

`ssh`

`ls`

`cd`

`file`

### 3. Methodology

- using the `ssh` command we establish connection to the server using `bandit4@bandit` and the password obtained by the last level.
- Once the connection is established we use `ls` command to check the files and directories we have in the current directory
- We change directories using `cd` to `inhere`
- using `file` with suitable parameters (`./*`) to list out the type of files stored in the directories
- Among all the listed files only one file has `ASCII text` content ,i.e., human-readable format. This file is `./-file07`.
- using `cat` we read the data of the file and thus access the password.


### 4. Syntax:

- `ssh bandit4@bandit.labs.overthewire@org -p 2220`
- `ls`
- `cd inhere`
- `ls`
- `file ./*`
- `cat ./-file07`

