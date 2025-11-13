# Bandit Level 1 → 2

**Date:** 2025-11-13  
**Tools Used:** ssh, cat  

---

## Problem
The password for the next level is stored in a file called - located in the home directory.
---

## Steps I Tried
- Connected to the server:  
  ```bash
  ssh bandit1@bandit.labs.overthewire.org -p 2220
- Password:"Look in file bandit0.md"

1.Ran ls - ; Found a file named "-"

2.Ran cat - ; Didnt not read

3.Found 2 Ways to deal with file named only "-"
  a.By using cat ./- ; Got Password
  Defined the file path
    . (a single dot): Represents the current working directory.
    ./: Specifies a file or folder located within the current directory.
    .. (two dots): Represents the parent directory, which is the directory one level above the current one.
    ../: Specifies a file or folder in the parent directory. 
  b.By using cat < - ; Got Password 
  Input redirection
    >: Redirects standard output (overwrites file).
    >>: Redirects and appends output to a file.
    <: Takes input from a file instead of the keyboard.
    2>: Redirects error messages to a file.
    &>: Redirects both standard output and error to a file.
<details>
  <summary> Click to reveal Password</summary>
   Password for bandit1: "263JGJPfgU6LtdEvgfWU1XP5yac29mFx"
</details>
  
## Lessons learned
- cat is simplest for reading text files.
- Some special Character file names are not readable directly hence should be avoided
- Learned about special characters, File path, Input redirection 
