# Bandit Level [1] -> Level [2]

- **Date:** 2026-08-10
- **Target:** Reading password from dashed file

---

### 1. Objective:

to locate and read the contents of the filsh e `-` containing the password for the next level

### 2. Commands used

`ls` `cat`

### 3. Learning Point

a dashed filename refers to a filename or directory whose name begins with a dash or hyphen

In unix and linux systems, these file cause errors because command line tools misinterpret the leading dash as a command flag or option instead of filename.

To safely open, read, or delete dashed files we have 2 primary techniques:

### A. Prefix with a Relative Path

- add a `./` prefix before the filename

### B. use the end-of-options delimiter

- a double dash (`--`) tells the command shell to stop looking for options or command flags
- 
### 4. Methodology and Syntax

- use the `ls` command to see if the file is present.
  
- once located we use `cat ./-` or `cat --` to read the file
