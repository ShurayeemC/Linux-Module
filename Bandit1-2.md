# OverTheWire Bandit - Level 1 to Level 2 Solution 🎮🔐

## The Goal 🎯  
To move from **Level 1** to **Level 2**, you need to find the password for the next level. Use the password from Level 0 to log into Level 1.  

---

## My Solution 💻  

### Step 1: Log into Level 1 🔑  
Use SSH to connect to the Level 1 server. Log in with the username `bandit1` and the password you got in Level 0 (**263JGJPfgU6LtdEvgfWU1XP5yac29mFx**).  

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```
When prompted, enter the password:

```bash
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
```

## Step 2: List the files in the directory 📂
Once you’re logged in, check the files in the directory by running:

```bash
ls
```
This will display

```bash
-
```

## Step 3: View the contents of the file 📖
In this level, you need to use input redirection (<) to read the contents of the file named -. Run this command:

```bash
cat < -
```
This will show the password for Level 2:

```bash
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
```
## Step 4: Log out when done 🛑
After you’ve found the password, exit the SSH session by typing

```bash
exit
```

## Takeaways 📚

Using SSH for secure connections 🔐
SSH is an important tool for securely accessing remote systems. Knowing how to log in and work on a remote server is an essential skill for IT and security professionals.

Using redirection to read files 🔄
The < symbol in Linux lets you pass the contents of a file to a command. This is useful for interacting with files that have special names, like - in this level.

Linux basics 🧭
Simple commands like ls and cat are fundamental for navigating and working with files in Linux. They’re useful not just in challenges like this but also in real-world Linux administration.

By completing this level, you’re improving your Linux command-line skills, which are vital for solving harder challenges and working on real-life projects. 🚀











