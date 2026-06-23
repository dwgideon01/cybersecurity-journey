# Day 2 - Linux Fundamentals

## Overview

Linux is one of the most important operating systems in cybersecurity. SOC Analysts use Linux to analyze logs, investigate incidents, manage systems, and automate tasks.

---

## pwd

### Description
The `pwd` command displays the current working directory.

### Example

```bash
pwd
```

### Output

```bash
/home/gideon
```

---

## ls

### Description
The `ls` command lists files and directories in the current location.

### Example

```bash
ls
```

---

## ls -la

### Description
The `ls -la` command lists all files, including hidden files, and shows detailed information such as permissions, ownership, and file size.

### Example

```bash
ls -la
```

---

## cat

### Description
The `cat` command displays the contents of a file.

### Example

```bash
cat notes.txt
```

---

## find

### Description
The `find` command searches for files and directories.

### Example

```bash
find ~ -name notes.txt
```

---

## grep

### Description
The `grep` command searches for specific words or patterns inside files.

### Example

```bash
grep "Failed" auth.log
```

### SOC Analyst Use Case

SOC Analysts use grep to search log files for suspicious activity such as:

```bash
grep "Failed password" auth.log
```

This can help identify brute-force login attempts.

---

## chmod

### Description
The `chmod` command changes file permissions.

### Example

```bash
chmod 600 secret.txt
```

### SOC Analyst Use Case

Proper file permissions help protect sensitive data from unauthorized access.

---

## chown

### Description
The `chown` command changes file ownership.

### Example

```bash
sudo chown gideon secret.txt
```

### SOC Analyst Use Case

During investigations, analysts check ownership of files to determine who created or modified them.

---

## Key Takeaways

- `pwd` shows the current directory.
- `ls` lists files and folders.
- `ls -la` shows hidden files and permissions.
- `cat` displays file contents.
- `find` searches for files.
- `grep` searches for text inside files.
- `chmod` changes permissions.
- `chown` changes ownership.

## Why This Matters In Cybersecurity

SOC Analysts regularly use Linux commands to:

- Investigate security incidents
- Search log files
- Identify suspicious activity
- Review file permissions
- Analyze compromised systems
