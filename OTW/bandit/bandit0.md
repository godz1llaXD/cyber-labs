# Bandit Level 0 → 1

**Date:** 2025-08-17  
**Tools Used:** ssh, cat  

---

## Problem
The password for the next level is stored in a file called `readme` in the home directory.  

---

## Steps I Tried
- Connected to the server:  
  ```bash
  ssh bandit0@bandit.labs.overthewire.org -p 2220
- Password:bandit0
  1.Ran ls - Found readme
  2.Ran cat readme - Got Password

<details>
  <summary> Click to reveal Password</summary>
### Password for bandit1: "ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If"
</details>
  
## Lessons learned
- Basic SSH login format (ssh user@host -p port).
- Always check home directory with ls.
- cat is simplest for reading text files.
