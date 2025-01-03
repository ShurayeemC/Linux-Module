# OverTheWire Bandit - Level 0 Solution 🎮🔐

## The Goal 🎯  
The challenge is to find the password for the next level. It’s stored in a file called `readme` on a remote server. You’re given login details for the `bandit0` user.  

---

## My Solution 💻  

### Step 1: Connect to the remote server 🌐  
We’ll use SSH (Secure Shell) to connect to the Bandit server. The username is `bandit0`, and the port is `2220`. Use the following command to log in:  

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

You’ll be asked for a password. You can find this on the OverTheWire website or in the challenge instructions.

### Step 2: List the files in the directory 📂
Once logged in, list the files in the current directory to find the readme file using this command:

```bash
ls
```

### Step 3: View the contents of the readme file 📖
Next, read the contents of the readme file to get the password using the cat command:

```bash
cat readme
```

### Step 4: Save the password for the next level 🔑
The password for the next level (bandit1) is:
ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

## What I Learned 📚
Using SSH for remote access 🌍
SSH is a secure way to connect to servers. It’s an important skill for anyone working with servers or managing remote systems.

Basic Linux commands 🧭
Commands like ls (list files) and cat (view file contents) are essential tools for navigating and managing files on Linux.

Problem-solving skills 🛠️
This level is a great reminder to take a simple, step-by-step approach:

Identify the problem (find and open the file).
Use the right tools (basic Linux commands).
