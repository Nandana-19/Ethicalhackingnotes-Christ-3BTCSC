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
DAY 4:


### 1. **IPv4 (Internet Protocol version 4)**

* **Definition**: IPv4 is the fourth version of the Internet Protocol used to identify devices on a network using an addressing system.
* **Address Format**: 32-bit address (e.g., `192.168.1.1`)
* **Total Addresses**: About **4.3 billion** unique addresses.
* **Structure**: Written in **dot-decimal notation** (four numbers separated by dots).
* **Limitation**: Because of the growing number of internet devices, IPv4 addresses are running out.

---

### 2. **IPv6 (Internet Protocol version 6)**

* **Definition**: IPv6 is the newer version of the Internet Protocol designed to replace IPv4.
* **Address Format**: 128-bit address (e.g., `2001:0db8:85a3:0000:0000:8a2e:0370:7334`)
* **Total Addresses**: Around **340 undecillion** (virtually unlimited).
* **Structure**: Written in **hexadecimal** and separated by colons.
* **Advantage**: Solves the IPv4 exhaustion problem and offers better routing and security features.

---

### 3. **MAC ID (Media Access Control Address)**

* **Definition**: A MAC ID (or MAC address) is a **unique hardware identifier** assigned to a network interface card (NIC) by the manufacturer.
* **Format**: 48-bit address, usually shown as `00:1A:2B:3C:4D:5E`
* **Purpose**: Used for identifying devices within a **local network (LAN)**.
* **Cannot Be Changed**: It's a physical address tied to the device (though it can be spoofed).

---

### 4. **TCP (Transmission Control Protocol)**

* **Definition**: TCP is a **connection-oriented** protocol that ensures **reliable communication** between two devices.
* **Features**:

  * Data is sent in a sequence.
  * Ensures data reaches correctly (error checking).
  * Slower but **more reliable**.
* **Examples**: Used in applications like **web browsing (HTTP/HTTPS)**, **email (SMTP)**, and **file transfers (FTP)**.

---

### 5. **UDP (User Datagram Protocol)**

* **Definition**: UDP is a **connectionless** protocol used for fast, **non-reliable communication**.
* **Features**:

  * No error checking or guaranteed delivery.
  * Much **faster** than TCP.
* **Examples**: Used in **video streaming**, **online gaming**, and **VoIP (Voice over IP)**.

---

### Comparison Table:

| Feature     | TCP                        | UDP                         |
| ----------- | -------------------------- | --------------------------- |
| Connection  | Connection-oriented        | Connectionless              |
| Speed       | Slower                     | Faster                      |
| Reliability | High (guaranteed delivery) | Low (no delivery guarantee) |
| Use Case    | Email, Web browsing        | Gaming, Streaming           |

---
### 🔍 **Reconnaissance in Cybersecurity**

**Definition**:
**Reconnaissance** is the **first phase** of the ethical hacking or cyberattack lifecycle. It involves **gathering information** about a target system, network, or organization **before launching an attack**. Think of it like a thief studying a building before breaking in.

---

### 🧠 **Purpose of Reconnaissance**

* To **understand the target's environment**
* Identify **vulnerabilities**, **open ports**, **IP addresses**, **technologies used**
* Reduce chances of **detection** during the actual attack
* Plan effective attacks or penetration tests

---

### 🛠️ **Types of Reconnaissance**

| Type              | Description                                                                                                                      |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| **Passive Recon** | Collecting info **without interacting** directly with the target. Example: looking at social media, WHOIS data, Google searches. |
| **Active Recon**  | Directly engaging with the target to gather information. Example: scanning networks, pinging devices, port scanning.             |

---

### 🔧 **Common Recon Tools**

| Tool             | Use                                                            |
| ---------------- | -------------------------------------------------------------- |
| **Nmap**         | Network scanning, open ports, services                         |
| **Wireshark**    | Packet analysis (network traffic)                              |
| **theHarvester** | Email, subdomain, and employee information gathering           |
| **Maltego**      | Visual link analysis for people, companies, domains, and IPs   |
| **Google Dorks** | Using advanced search techniques to find sensitive information |

---

### 🧾 **Examples of Information Collected**

* IP address ranges
* Subdomains
* Open ports
* Software versions
* Employee names or emails
* DNS records

---

### ⚠️ **Why It Matters**

In ethical hacking, reconnaissance helps in:

* Finding weak points before an attacker does
* Strengthening defenses proactively
* Simulating real-world attack planning for better security

---
1. Low Privilege User
Definition:
A low privilege user is an account configured with minimal permissions necessary to perform its intended tasks. This is a core part of the Principle of Least Privilege (PoLP), which ensures that users can only access what they strictly need.

Characteristics:

Cannot install software or change system-wide configurations.

Limited access to files and directories (e.g., only their home folder).

Restricted from managing other users or system processes.

Cannot access sensitive system logs or security settings.

Examples:

Windows: Standard User account vs. Administrator.

Linux/Unix: Non-root user (e.g., student account with no sudo rights).

Corporate Environment: Employee account without admin rights on their workstation.

Security Benefits:

Reduces damage in case of account compromise.

Prevents unauthorized installation of malicious software.

Limits insider threats by restricting unnecessary access.

Risks:

Even with low privileges, attackers can:

Steal accessible data.

Use the account as a foothold to attempt privilege escalation.

Participate in lateral movement within the network.

2. SOC (Security Operations Center)
Definition:
A Security Operations Center (SOC) is a dedicated team and facility that monitors an organization’s IT infrastructure to detect, analyze, respond to, and prevent cybersecurity incidents.

Key Objectives:

Continuous monitoring: 24/7 real-time observation of security events.

Incident detection: Identifying unusual or malicious activity.

Incident response: Containing and mitigating active threats.

Threat intelligence: Using external and internal sources to anticipate attacks.

Compliance: Ensuring security standards meet legal and regulatory requirements.

SOC Structure:

Tier 1 – Alert Monitoring & Triage

Receives alerts from SIEM systems.

Filters false positives.

Tier 2 – Incident Investigation

Deep analysis of suspicious events.

Determines impact and scope.

Tier 3 – Threat Hunting & Response

Proactive search for hidden threats.

Develops detection rules.

SOC Manager

Oversees operations.

Coordinates incident communication.

Common SOC Tools:

SIEM: Splunk, IBM QRadar, ArcSight.

Endpoint Detection & Response (EDR): CrowdStrike, SentinelOne.

Intrusion Detection Systems (IDS): Snort, Suricata.

Threat Intelligence Platforms (TIPs).

Example Workflow:

SOC receives alert from SIEM.

Analyst checks logs for unusual login activity.

Incident escalated if suspicious.

Response team isolates affected system.

Incident is documented for future prevention.

3. Data Exfiltration
Definition:
Data exfiltration is the unauthorized transfer of sensitive data from within an organization’s network to an external location controlled by an attacker.

Common Targets:

Personally Identifiable Information (PII).

Financial data.

Intellectual property.

Login credentials.

Methods of Data Exfiltration:

Manual methods: Using USB drives, CDs, smartphones.

Over the network:

Emailing to personal accounts.

Uploading to cloud storage (Google Drive, Dropbox).

Using file transfer protocols (FTP, SFTP).

Covert channels:

DNS tunneling.

Embedding data in images (steganography).

HTTPS traffic to hide malicious transfers.

Causes:

Insider threats.

Compromised credentials.

Malware infections.

Exploiting unsecured APIs.

Detection Techniques:

Monitoring unusual network traffic volume.

Detecting uploads to unknown domains.

Data Loss Prevention (DLP) systems.

Prevention:

Enforce encryption for sensitive data.

Use DLP solutions.

Apply strict access controls.

Employee awareness training.

4. Privilege Escalation
Definition:
Privilege escalation occurs when an attacker gains higher-level permissions than initially granted, allowing them to perform unauthorized actions.

Types:

Vertical Privilege Escalation:
Gaining higher privileges than assigned (e.g., user → admin/root).

Horizontal Privilege Escalation:
Accessing resources of another account with the same privilege level (e.g., user A accessing user B’s emails).

Techniques:

Exploiting unpatched software vulnerabilities.

Weak or misconfigured file permissions.

Credential theft (pass-the-hash, keylogging).

Exploiting SUID binaries in Linux.

DLL injection or malicious service creation in Windows.

Example Attack Path:

Attacker compromises a low privilege account.

Exploits vulnerability to gain administrator rights.

Accesses sensitive files or deploys malware.

Potentially performs data exfiltration.

Mitigation:

Apply timely patches and updates.

Enforce PoLP for all accounts.

Monitor logs for unusual privilege changes.

Use Multi-Factor Authentication (MFA).

Implement Privileged Access Management (PAM) tools.

How They Connect in a Real Attack
Initial Access – Attacker compromises a low privilege user (via phishing or stolen credentials).

Privilege Escalation – Attacker gains higher privileges to access more resources.

Data Exfiltration – Sensitive files are copied to attacker-controlled servers.

SOC Detection – SOC detects unusual activity, investigates, and responds





