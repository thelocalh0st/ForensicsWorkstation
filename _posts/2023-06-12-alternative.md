---
layout: post
author: sujay adkesar
tags: [SIFT-alternative, BuildYourWorkstation]
---

<link href="https://fonts.googleapis.com/css2?family=Lato&display=swap" rel="stylesheet">

<br>
<div class="eleven">
  <h1 style="color:cyan;">Workstation Setup Instructions</h1>
</div>
<br>


<iframe width="560" height="315" style="display: block; margin: auto;" src="https://www.youtube.com/embed/BmFZDgMEtEY?si=ZbW9QXShN8FrT5Gy" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## 1) Install a Hypervisor

For an overview of virtualization options as well as useful information regarding VirtualBox see  [Virtualization Primer](https://bluecapesecurity.com/build-your-lab/virtualization/).

**1.1 Download and install a hypervisor**:  [VirtualBox](https://www.virtualbox.org/wiki/Downloads)  (recommended)

**Note**: At the time of writing,  [VirtualBox and others only support WSL1](https://docs.microsoft.com/en-us/windows/wsl/faq#will-i-be-able-to-run-wsl-2-and-other-3rd-party-virtualization-tools-such-as-vmware--or-virtualbox-), which is important to consider, but OK for our purposes.

## 2) Install Windows Guest VM

You can find various and free Windows trial versions in the [Microsoft Evaluation Center](https://www.microsoft.com/en-us/evalcenter)!

We recommend downloading a  Windows Server 2019 VHD  version, as it provides the best performance and the setup process for WSL1 is easier than with others. It’s also the quickest way to download a ready-to-go VHD, which skips the need to install the operating system from an ISO.

**2.1) Download the Guest VM**

a)  [Windows 2019 Server ISO or VHD](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)  from the Evaluation Center ([VHD direct link](https://go.microsoft.com/fwlink/p/?linkid=2195334)).

b) Alternatively, you can download other versions. However, carefully read the instructions in the WSL setup section below!

-   [This post on the Microsoft Tech Community page](https://techcommunity.microsoft.com/t5/windows-11/accessing-trials-and-kits-for-windows-eval-center-workaround/m-p/3361125)  contains direct links to all available ISOs for Windows 10/11 and Windows server 2019/2022[](https://developer.microsoft.com/en-us/windows/downloads/virtual-machines/)

Important to note that the Windows client comes with a 90-day and Windows server with a 180-day evaluation period. There are ways to extend the period for some systems by  [re-arming](https://techtrix.co/how-do-i-extend-windows-10-enterprise-evaluation/)  them.

**2.2) Install a new Windows VM**

_For detailed instructions see the setup guides for VirtualBox and a [Windows 10 VM](https://bluecapesecurity.com/build-your-lab/basic-lab/)  or a  [Windows 2019 Server.](https://bluecapesecurity.com/build-your-lab/medium-lab/)_

1.  VM requirements:
    -   100 GB disk – dynamically allocated! That way the disk is kept small and grows larger when needed. However, it can’t go beyond the initial size. So make sure to choose the right size based on the expected amount of data to be analyzed.
    -   4+ GB RAM
    -   2 or more CPUs
    -   NAT Networking Mode
    -   Additionally, install VirtualBox Guest Additions and enable features such as Drag & Drop, bi-directional clipboard, and folder sharing with the host in the VMs settings.
2.  Install Windows from the ISO.
3.  When finished, shut down the system and create a snapshot.

## 3) Enable Windows Subsystem for Linux (WSL) and Install Ubuntu

As mentioned above, VirtualBox does not support WSL2. It is important to read the respective instructions carefully to set up a Ubuntu subsytem using WSL1 on your Windows VM.

a)  [Microsoft Installation Guide for Windows Server](https://docs.microsoft.com/en-us/windows/wsl/install-on-server)

-   Open PowerShell as Administrator and run the following command:

Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux

-   Download the Ubuntu 20.04 Distribution  [here](https://docs.microsoft.com/en-us/windows/wsl/install-manual#downloading-distributions)
-   When downloaded, rename the package from .appxbundle to .zip and extract the archive
-   Install the x64.appx package contained within the archive using the following PowerShell command (as administrator!):

Add-AppxPackage .\Ubuntu_2004.4.2.0_x64.appx

-   Reboot the system
-   Finish the installation by opening “Ubuntu” in your Start Menu and setting up a user account when asked for it.

b) Other Windows Versions

-   Windows 10/11 from ISO
    -   Use the  [manual steps in for older versions guide](https://docs.microsoft.com/en-us/windows/wsl/install-manual)  to set up WSL1 on your Windows system.  **Do NOT upgrade to WSL2 and skip steps 2 to 5!**
    -   [Install Ubuntu from the Microsoft store](https://docs.microsoft.com/en-us/windows/wsl/install-manual#step-6---install-your-linux-distribution-of-choice)
-   Windows 11 Developer VM
    -   This version comes with WSL2 and Ubuntu out of the box.  [You need to downgrade to WSL1.](https://github.com/MicrosoftDocs/WSL/issues/590)

c) WSL Troubleshooting

-   Do not use the new Microsoft command “wsl –install”, since this is going to install WSL2, which won’t work with VirtualBox.
-   To check if you have WSL2 installed type “wsl –version” in PowerShell. It will show several options for using WSL with version 2 if you have it. Otherwise, for version 1 you will only see a limited help menu.
-   If you installed WSL2, you need to downgrade to WSL1 before you can install any Linux environment: “wsl –set-default-version 1”

## 4) Configure the Windows Environment

The following settings are digital forensics best-practices that should be considered when setting up a forensic workstation:

1.  Set the  **time zone**  to UTC – important!
    -   This is a general best practice for conducting forensic analysis and ensures a standard time zone is being used across all tools. It also helps to correlate events that possibly happened across different time zones or where the origin is not clear.
2.  Configure Windows Explorer to  **show hidden files**. This enables viewing file types that a relevant in forensic analysis such as NTFS metadata, etc.
    -   Open File Explorer -> View -> check “Hidden items” and “File name extensions”.
3.  Create a  **“C:\Cases”** and a  **“C:\Tools” folder**  for evidence data and tools respectively.
    -   Having your folders in the root of your file system saves you from typing long paths on the command line when using them. You may also want to add a shortcut to your Desktop.
4.  Configure  **Microsoft Defender** to avoid interference with evidence or tools.
    -   Open Virus & threat protection settings.
    -   Disable Defender’s “Real-time protection” when needed for a temporary period of time. If you want to  [permanently turn off real-time protection](https://bluecapesecurity.com/prepare-your-target-system/)  you need to disable it via GPO as described in the next section.
    -   Disable “Cloud-delivered protection” and “Automatic sample submission”, which only needs to be done once.
    -   Exclude your working directories e.g. “C:\Cases” and “C:\Tools” from Defender’s virus and threat protection scanning. That way Defender won’t detect and remove important files during an investigation. Go to “Exclusions” -> “Add an exclusion” -> “Folder”.


## 5) Download and Install Forensic Tools


<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi0.wp.com%2Fdigitalforensicsinvestigations.uk%2Fwp-content%2Fuploads%2F2018%2F02%2FCForensicsLab_orig.jpg%3Fresize%3D768%252C531%26ssl%3D1&f=1&nofb=1&ipt=d9d18c2798254f63543ae15e18aa02f41bf6f7e7f03dea78882bde352ca2bc6e&ipo=images" style="display: block; margin: auto;">

<br>

1. **Autopsy**
   - Autopsy is an open-source digital forensics platform that supports the analysis of disk images, file carving, and keyword searching.

2. **The Sleuth Kit (TSK)**
   - TSK is a library and command-line tool that allows forensic investigators to analyze disk images and recover evidence.

3. **EnCase**
   - EnCase by Guidance Software is a widely used commercial digital forensics tool that provides features for disk analysis, evidence acquisition, and forensic reporting.

4. **Forensic Toolkit (FTK)**
   - FTK is a comprehensive digital forensics tool that helps in analyzing email, computer, and mobile data. It provides advanced search and data recovery capabilities.

5. **Volatility**
   - Volatility is an open-source memory forensics framework that assists in the analysis of memory dumps. It helps in extracting information about running processes and system interactions.

6. **Wireshark**
   - Wireshark is a powerful network protocol analyzer. It is used for capturing and analyzing the data traveling back and forth on a network, which can be crucial for investigating network-based incidents.

7. **HashCalc**
   - HashCalc is a tool used for calculating hash values of files. Hash values are crucial for verifying the integrity of evidence during forensic analysis.

8. **RegRipper**
   - RegRipper is a tool for parsing Windows Registry hives. It helps in extracting valuable information from the Registry, which can be important for forensic investigations.

9. **Open Source Digital Forensics (OSDF)**
   - OSDF is a collection of various open-source digital forensics tools, providing a comprehensive suite for investigators.

10. **NetworkMiner**
    - NetworkMiner is a network forensic analysis tool that helps in capturing and analyzing network traffic. It can extract files, emails, and other artifacts from network traffic.

11. **Paladin Forensic Suite**
    - Paladin is a Linux distribution built for digital forensics and incident response. It includes a variety of tools for data acquisition, disk imaging, and analysis.

12. **X-Ways Forensics**
    - X-Ways Forensics is a powerful and efficient computer forensics tool that allows investigators to conduct in-depth analysis of disk images, partitions, and file systems.

13. **Snort**
    - Snort is an open-source intrusion detection system that can be used for monitoring and analyzing network traffic. It aids in identifying and responding to security incidents.

14. **Ghiro**
    - Ghiro is an open-source digital image forensics tool that helps in analyzing and extracting information from images. It can be useful for uncovering hidden details or alterations.

15. **Cellebrite UFED**
    - Cellebrite UFED is a commercial mobile forensics solution designed to extract and analyze data from mobile devices, including smartphones and tablets.

Before using any of these tools, it's essential to be aware of legal and ethical considerations and ensure that their usage complies with applicable laws and regulations. Additionally, the specific tools chosen may depend on the nature of the investigation and the types of devices involved.
