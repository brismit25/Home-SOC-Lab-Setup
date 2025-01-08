---
layout: default
---

# Windows 11 Setup

## Step 1: Download Windows 11

> Download [Windows 11 64 bit](https://www.microsoft.com/en-us/software-download/windows11)

<br>

## Step 2: Create new VM

> Launch Oracle VBM and select "New"
>
> <img src="assets/Win11/Screenshot 2025-01-02 065719.png">
>
> Follow along with below images on completing the VM setup
>
> <img src="assets/Win11/Screenshot 2025-01-02 072028.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 072541.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 073024.png">

<br>

## Step 3: Network Settings

> Select the Windows 11 VM's settings and then network
>
> <img src="assets/Win11/Screenshot 2025-01-02 073758.png">
>
> In Network settings configure the following
> 
> <img src="assets/Win11/Screenshot 2025-01-02 073931.png">

<br>

## Step 4: Installing Windows 11 on VM

> Launch the Windows 11 VM
>
> <img src="assets/Win11/Screenshot 2025-01-02 074612.png">
>
> Once VM launches, follow through the Windows 11 Installation process
>
> <img src="assets/Win11/Screenshot 2025-01-02 074918.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 074927.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 075157.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 075300.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 075526.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 075607.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 075656.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 075748.png">
>
> After Windows 11 installs, the system will reboot
>
> After the reboot, follow through the Windows Setup process
>
> On the select country or region screen, push Shift-F10 to open Command Prompt. In Command Prompt enter OOBE\BYPASSNRO and the system will reboot (this bypasses the Network requirement and Microsoft account sign-in)
>
> <img src="assets/Win11/Screenshot 2025-01-02 081337.png">
>
> 
> <img src="assets/Win11/Screenshot 2025-01-02 082254.png">
>
> Complete the Local Account Setup
>
> <img src="assets/Win11/Screenshot 2025-01-02 082628.png">

<br>

## Step 5: Configuring Windows 11

> Login to Windows 11
>
> Open Network & Internet Settings
>
> <img src="assets/Win11/Screenshot 2025-01-02 083447.png">
>
> Follow below images to configure Window 11 IPv4 Network settings
>
> <img src="assets/Win11/Screenshot 2025-01-02 083544.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 083613.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 083732.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 084127.png">
>
> Assign a Static IP, Subnet, and Gateway ("LAN" IP Address from pfSense VM). The Preferred DNS server will be the IP Address of the Windows Server machine, then another known DNS server (ex. Google's DNS Server)
>
> <img src="assets/Win11/Screenshot 2025-01-02 084716.png">
>
> Next rename Windows 11 computer and reboot
>
> <img src="assets/Win11/Screenshot 2025-01-02 092417.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 092437.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 092446.png">
>
> After the reboot is complete, follow below to add computer to the domain created on Windows Server
>
> <img src="assets/Win11/Screenshot 2025-01-02 092931.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 093014.png">
>
> <img src="assets/Win11/Screenshot 2025-01-02 093318.png">

<br>

# _Windows 11 Setup is complete_

<br>

[Back To Project's Homepage](https://brismit25.github.io/Home-SOC-Lab-Setup/)
