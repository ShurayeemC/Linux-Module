# OverTheWire Bandit - Level 2 to Level 3 Solution 🎮🔐

## The Goal 🎯  
To move from **Level 2** to **Level 3**, you need to find the password for the next level. The password is stored in a file with spaces in its name, which requires special handling. Use the password from Level 1 to log into Level 2.  

---

## My Solution 💻  

### Step 1: Log into Level 2 🔑  
Use SSH to connect to the Level 2 server. Log in with the username `bandit2` and the password from Level 1 (**MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx**).  

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```
When prompted, enter the password:

```bash
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
```

## Step 2: List the files in the directory 📂
After logging in, list the files in the current directory using the ls command:

```bash
ls
```

This will show a file with spaces in its name.

## Step 3: Read the contents of the file 📖
To read the file, you need to handle the spaces in its name. Wrap the filename in quotes (either double " or single ' quotes):

```bash
cat "spaces in this filename"
```
This will display the password for the next level:

```bash
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
```
## Step 4: Log out when done 🛑
Once you’ve saved the password, exit the session by typing:

```bash
exit
```












