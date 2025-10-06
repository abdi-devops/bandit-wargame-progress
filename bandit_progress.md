## Level 0
**Goal:** SSH into bandit0@bandit.labs.overthewire.org on port 2220

## Level 0 → Level 1
**Goal:** Read a file named `readme`.  
**Commands Used:**  
```bash
ls
cat readme
```

## Level 1 → Level 2
**Goal:** Read a file named `-`.  
**Commands Used:**  
```bash
ls
cat ./-
```
**Lesson Learned:** Use ./ to reference filenames that look like flags (e.g. -).

## Level 2 → Level 3
**Goal:** Read a file named `--spaces in this filename`.  
**Commands Used:**  
```bash
ls
cat ./'--spaces in this filename'
```
**Lesson Learned:** Quotes can be used to escape spaces in filenames. Backslashes may also be used.

## Level 3 → Level 4
**Goal:** Read a hidden file  
**Commands Used:**  
```bash
ls
cd inhere
ls
ls -a
cat ...Hiding-From-You
```

## Level 4 → Level 5
**Goal:** Find the human readable file
**Commands Used:**
```bash
ls
cd inhere
ls
file ./*
cat ./-file07
```

## Level 5 → Level 6
**Goal:** Find the file that has the following properties:
human-readable
1033 bytes in size
not executable
**Commands Used:**  
```bash
```
**Lesson Learned:** 
