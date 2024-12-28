# OverTheWire Bandit - Level 4 to Level 5 Solution 🎮🔐

## The Goal 🎯:
To move from **Level 4** to **Level 5**, you need to find the password for the next level. This involves exploring files and using the `man` page to learn about the `file` command. One of the files contains the password.

---

## My Solution 💻:

### Step 1: Log in to the next level using SSH 🔑
To access Level 4, connect to the server via SSH. Use the username `bandit4` and the password from the previous level (`4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw`).

```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```

You’ll be asked for the password. Enter the password you got from Level 4:

```bash
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
```

## Step 2: List the files in the directory 📂
Once logged in, use the ls command to list the files in the current directory.

```bash
ls
```
You should see a directory called inhere.

## Step 3: Go to the inhere directory 📂
Change to the inhere directory with the cd command.

```bash
cd inhere
```

## Step 4: Check the man page for the file command 📖
Use the man command to view the manual for the file command. This command helps you identify file types, which will help in your next steps.

## Step 5: List all files with details using ls -la 📑
Use the ls -la command to list all the files in the inhere directory, including hidden files, along with information about their permissions and types.

Output:

```bash
total 48
drwxr-xr-x 2 root    root    4096 Sep 19 07:08 .
drwxr-xr-x 3 root    root    4096 Sep 19 07:08 ..
-rw-r----- 1 bandit5 bandit4   33 Sep 19 07:08 -file00
-rw-r----- 1 bandit5 bandit4   33 Sep 19 07:08 -file01
-rw-r----- 1 bandit5 bandit4   33 Sep 19 07:08 -file02
-rw-r----- 1 bandit5 bandit4   33 Sep 19 07:08 -file03
-rw-r----- 1 bandit5 bandit4   33 Sep 19 07:08 -file04
-rw-r----- 1 bandit5 bandit4   33 Sep 19 07:08 -file05
-rw-r----- 1 bandit5 bandit4   33 Sep 19 07:08 -file06
-rw-r----- 1 bandit5 bandit4   33 Sep 19 07:08 -file07
-rw-r----- 1 bandit5 bandit4   33 Sep 19 07:08 -file08
-rw-r----- 1 bandit5 bandit4   33 Sep 19 07:08 -file09
```
## Step 6: Use the file command to check the file types 🔍
Use the file command to check the type of each file.

```bash
file ./*
```

The output will look like this:

```bash
./-file00: data
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data
```
## Step 7: View the content of the file with text data 📖
The file -file07 is identified as "ASCII text," so it contains readable content. Use the cat command to view the file and find the password.

```bash
cat ./-file07
```

Output:

```bash
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
```

## Step 8: Log Out
After getting the password for Level 5, exit the SSH session by typing:

```bash
exit
```

## Takeaways 📚:
SSH for Secure Access 🔐: SSH is essential for securely connecting to remote systems. It will be used throughout the Bandit game and in real-world tasks.

Using the file Command 📑: The file command is helpful for determining file types, especially when dealing with files that don't have obvious extensions.

File Permissions 🔒: The ls -la command shows file permissions and ownership. Understanding these permissions is important for working with Linux systems securely.

By completing this level, you're improving your skills in using Linux commands to explore and manage files and gaining a better understanding of system concepts like file types and permissions. 🚀









