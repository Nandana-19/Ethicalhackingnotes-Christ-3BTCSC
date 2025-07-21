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

