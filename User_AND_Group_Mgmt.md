# Linux USER MANAGEMENT — FRIENDLY EDITION

As a linux admin in your org you are expected to manage the user access of the employees which includes CRUD operations of the user and
you will be administrating the users, their activites and lot more. So learn these commands and when you use them at your work..come thank me :p

<-------------------------------------USERS / USER MANAGEMENT--------------------------->

Imagine a new employee had joined your team..and your manager/lead asks you to provide the access on a server for your team mate--then this is how you do it...and then the guide continues with further steps involved in usermanagement.

**useradd username** →creates a new user

```bash
useradd username
useradd amree
```

**passwd username** → set password for that user

```bash
passwd username
passwd amree
```

**How to check if user got created?**

```bash
cat /etc/passwd
```

**Wanna see encrypted passwords?**

```bash
cat /etc/shadow
```

⚠️ note: You CANNOT view the original password. It’s one-way encrypted. Forget it → set a new one.

**Create user WITH home directory**

```bash
adduser username
adduser amrita
```

**Why do we even need user management re?**

- Accountability
- Security
- No random user gets root access
- Server stays safe 🛡️

**Who am I?**

```bash
whoami
```

---

<------------------------👥 GROUPS / GROUP MANAGEMENT----------------------->

You're the **Group Manager Bro** now 🤓

Why groups?  
Managing 5–10 users is easy.  
Managing 100s of users individually = pain 😭  
Groups save the day like Batman 🦇

Examples:

- Devs → devgroup
- QEs → qe group

Group = common permissions for all.  
Change once → applies to everyone 🎯

**Create a group**

```bash
groupadd group_name
groupadd devgroup
```

**Check groups**

```bash
cat /etc/group
```

**Add user to a group**

```bash
usermod -aG group_name username
usermod -aG devgroup amree_dev
```

Bro tip:  
Admins share **IP + username + password** safely with new users.

---

<-----------------🔐 SSH (Secure Shell)-------------------->

New user got access… cool!  
But how do they log in? → SSH bro 😎

A service called **sshd** runs on Linux machines → allows remote login.

Windows → Git Bash  
Mac/Linux → Terminal

**SSH command**

```bash
ssh username@ip_address
ssh amrita@10.x.x.x
```

Enter password → You're inside 🚀

---

<-------📁 FILE MANAGEMENT IN LINUX-------->

**List all files**

```bash
ls
```

**Change directories**

```bash
cd path
cd /home/amree
```

**Go back one directory**

```bash
cd ..
```

**Go back multiple directories**

```bash
cd ../../..
```

---

### Create a directory

```bash
mkdir directory_name
mkdir server_details
```

### Delete an EMPTY directory

```bash
rmdir directory_name
rmdir amree_dir
```

### Create a file

```bash
touch file_name
touch file1.txt
touch config.conf
```

### Delete a file

```bash
rm -f file_name
rm -f file1.txt
```

### Delete a directory WITH all its content

```bash
rm -rf directory_name
```

`-r` = recursive  
`-f` = force  
⚠️ Be careful — this is the nuclear bomb of Linux commands 💣

---

🔥 **SUMMARY**  
You just learned Linux basics with full swag:  
Users ✔️ Groups ✔️ SSH ✔️ Files ✔️
