# MyNOTES
Setting Up Kali Linux on Windows Using VirtualBox
Planning to run Kali Linux on your Windows machine? Follow this guide step-by-step to get everything up and running using Oracle VirtualBox.

Required Downloads
Before beginning, make sure you have the following files:

Kali Linux VirtualBox Image:
https://cdimage.kali.org/kali-2025.2/kali-linux-2025.2-virtualbox-amd64.7z

Oracle VirtualBox:
https://download.virtualbox.org/virtualbox/7.1.12/VirtualBox-7.1.12-169651-Win.exe

7-Zip File Archiver:
https://www.7-zip.org/a/7z2500-x64.exe

 Step 1: Installing Oracle VirtualBox
Double-click the downloaded VirtualBox-7.1.12-169651-Win.exe file.

Click Yes if Windows asks for admin permission.

In the setup window, click Next to continue.

Leave the default settings as-is on the Custom Setup screen, and click Next.

If a warning about "Network Interfaces" pops up, click Yes to proceed.

If the installer warns about missing dependencies, click Yes again.

Click Install to begin installation.

Once it finishes, click Finish to launch VirtualBox.

 TROUBLESHOOTING INSTALLATION ISSUES
🔹 Problem: Missing Microsoft Visual C++ Redistributable
If VirtualBox doesn’t open or throws an error, you may need a system library.

Download and install this file:
🔗 https://aka.ms/vs/17/release/vc_redist.x64.exe

Then restart the VirtualBox installation.

Inside BIOS, find Virtualization Technology or SVM Mode under Advanced Settings, and enable it.

 Step 2: Installing 7-Zip
Right-click the downloaded 7z2500-x64.exe file and choose Run as Administrator.

When the installer opens, click Install.

After it’s done, click Close.

 Step 3: Extract the Kali Linux Image
Navigate to the folder where you downloaded the .7z file for Kali.

Right-click the file, go to 7-Zip > Extract Here.

This may take a few minutes. Once finished, you'll see the extracted VM files.

 Step 4: Load Kali into VirtualBox
(Optional but recommended) Move the extracted Kali files to a separate partition with ~10–15 GB free space.
A tutorial if needed: https://www.youtube.com/watch?v=HGqo17dGk0E

Inside the extracted folder, locate the file with a .vbox extension — this is the VirtualBox machine definition file.

Double-click that file. It will automatically open in Oracle VirtualBox.

Click the Start button to boot up Kali Linux. First-time startup may take some time.

When prompted for login details, use:

Username: kali

Password: kali

DAY 3:

## 🗂️ **1. File & Directory Management**

| **Command**                  | **Description**                                     |
| ---------------------------- | --------------------------------------------------- |
| `ls`                         | Lists files and directories in the current location |
| `ls -l`                      | Lists with details (size, date, permissions)        |
| `cd foldername`              | Changes directory to the specified folder           |
| `cd ..`                      | Goes up one directory level                         |
| `pwd`                        | Displays the current directory path                 |
| `mkdir foldername`           | Creates a new folder                                |
| `rm filename`                | Deletes the specified file                          |
| `rm -r foldername`           | Deletes a folder and its contents                   |
| `touch file.txt`             | Creates an empty file named `file.txt`              |
| `cp source.txt dest.txt`     | Copies file from source to destination              |
| `mv oldname.txt newname.txt` | Renames or moves a file                             |

---

## 📄 **2. Viewing & Editing Files**

| **Command**           | **Description**                              |
| --------------------- | -------------------------------------------- |
| `cat file.txt`        | Displays contents of a file                  |
| `less file.txt`       | Opens file for scrolling (press `q` to quit) |
| `nano file.txt`       | Opens file in the Nano text editor           |
| `vim file.txt`        | Opens file in Vim editor (advanced)          |
| `head -n 10 file.txt` | Shows the first 10 lines of a file           |
| `tail -n 10 file.txt` | Shows the last 10 lines of a file            |

---

## 🔧 **3. System & Package Management**

| **Command**               | **Description**                             |
| ------------------------- | ------------------------------------------- |
| `sudo`                    | Runs a command with root (admin) privileges |
| `apt update`              | Updates the list of available packages      |
| `apt upgrade`             | Installs the latest versions of packages    |
| `apt install packagename` | Installs a new software package             |
| `apt remove packagename`  | Removes an installed package                |
| `clear`                   | Clears the terminal screen                  |
| `reboot`                  | Reboots the system                          |
| `shutdown now`            | Immediately shuts down the system           |

---

## 🔍 **4. Searching & Permissions**

| **Command**                | **Description**                                  |
| -------------------------- | ------------------------------------------------ |
| `find . -name "file.txt"`  | Searches for `file.txt` in the current directory |
| `grep "word" file.txt`     | Searches for "word" in `file.txt`                |
| `chmod 755 file.sh`        | Changes permissions of a file                    |
| `chown user:user file.txt` | Changes the ownership of a file                  |

---

## 📊 **5. System Information**

| **Command**          | **Description**                              |
| -------------------- | -------------------------------------------- |
| `uname -a`           | Shows system information (kernel, OS)        |
| `top` / `htop`       | Shows running processes and system usage     |
| `df -h`              | Displays disk usage in human-readable form   |
| `free -h`            | Shows memory (RAM) usage                     |
| `whoami`             | Shows the current logged-in user             |
| `ifconfig` or `ip a` | Displays network interfaces and IP addresses |

---

##  **6. Shortcuts & Tips**

| **Key/Command** | **Action**                               |
| --------------- | ---------------------------------------- |
| `Tab`           | Auto-completes file/folder names         |
| `Ctrl + C`      | Cancels a running command                |
| `Ctrl + L`      | Clears the screen (like `clear`)         |
| `Ctrl + D`      | Logs out of the current terminal session |

Here’s a clean **table with brief descriptions** for the Linux commands you listed, along with a small introductory paragraph:

---

### 📝 **Introduction**

Linux provides a powerful terminal where you can manage files, processes, and the system using simple commands. Below is a list of essential Linux commands that every beginner should know. These commands help with navigation, file operations, permissions, and system monitoring.

---

### **Linux Commands Table**

| **Command** | **Description**                                           |
| ----------- | --------------------------------------------------------- |
| `ls`        | Lists files and folders in the current directory          |
| `cd`        | Changes the current directory                             |
| `pwd`       | Prints the current working directory path                 |
| `mkdir`     | Creates a new directory                                   |
| `rmdir`     | Deletes an empty directory                                |
| `touch`     | Creates an empty file                                     |
| `rm`        | Deletes files or directories (`-r` for folders)           |
| `cp`        | Copies files or directories                               |
| `mv`        | Moves or renames files and directories                    |
| `man`       | Opens the manual/help page for a command (e.g., `man ls`) |
| `echo`      | Prints text to the terminal (e.g., `echo Hello`)          |
| `kill`      | Sends a signal (usually stop) to a process by its PID     |
| `chmod`     | Changes file or folder permissions                        |
| `chown`     | Changes the owner of a file or folder                     |
| `ps`        | Shows current running processes                           |
| `top`       | Real-time display of processes and system usage           |
| `df`        | Shows disk space usage on mounted file systems            |


