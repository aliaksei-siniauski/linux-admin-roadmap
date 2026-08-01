# Week 01 - Linux Basics Exercises

## Goal

Practice the basic Linux commands used for navigation, file management, file reading, searching, and disk usage.

---

# Exercise 1 - Navigation

## Task

Display:

Current user
Current directory
Files in the current directory

## Commands Used

```bash
whoami
pwd
ls -la
```

## What I Learned

`whoami` - displays the current user
`pwd` - displays the current working directory
`ls -la` - lists all files, including hidden files

# Exercise 2 - Create Directories

## Task

Create the following directory structure:

```
linux-lab/
├── documents
├── scripts
├── logs
└── backups

```

## Commands Used

```bash
mkdir -p linux-lan/{documents,scripts,logs,backups,configs tmp data reports}
```

## What I Learned

`mkdir` - creates directories.
Linux allows nested directory structures

---


# Exercise 3 - Create Files

## Task

Create the following files:

- notes.txt
- server.log
- backup.txt
- script.sh

## Command Used

```bash
touch notes.txt touch server.log touch backup.txt touch script.sh 
```

## What I Learned

`touch` - creates empty files.
It can also update a file's timestamp.


# Exercise 4 - Copy and Move Files

## Task
Copy:

- notes.txt → backups/

Move:

- backup.txt → documents/

## Commands Used

```bash
cp notes.txt backups/
mv backup.txt documents/
```

## What I Learned

`cp` - copies files.
`mv` - moves or renames files.

---

# Exercise 5 - Remove Files

## Task

Delete:

- server.log

## Commands Used

```bash
rm logs/server.log
```

## What I Learned

`rm` - permanently deletes files.
`rm -r` - delete eveything inside directory

---

# Exercise 6 - Read Files

## Task

Add text to notes.txt and display it.

## Commands Used

```bash
echo "Linux is awesome!" > notes.txt

cat notes.txt

head notes.txt

tail notes.txt

less notes.txt
```

## What I Learned

`cat` - displays a file.
`head` - shows the first lines.
`tail` - shows the last lines.
`less` - allows interactive viewing.

---

# Exercise 7 - Search Files

## Task

Find:

- script.sh

Locate:

- bash
- python

## Commands Used

```bash
find . -name script.sh
which bash
whereis python
```

## What I Learned

`find` - searches for files
`which` - locates executables
`whereis` - shows executable, source, and manual locations

---

# Exercise 8 - Disk Usage

## Task

Display disk usage information.

## Commands Used

```bash
df -h
du -sh linux-lab
```

## What I Learned

`df` - displays filesystem disk usage.
`du` - displays the size of files and directories.

---

# Exercise 9 - Measure Execution Time

## Task

Measure how long it takes to list all files.

## Commands Used

```bash
time ls -la
```

## What I Learned

`time` - measures the execution time of a command.

---

## Week 01 Summary

### Skills Practiced

- Linux navigation
- File management
- Reading files
- Searching files
- Disk usage
- Measuring command execution time
