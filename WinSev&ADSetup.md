---
layout: default
---

# Windows Server and Active Directory Setup

## Step 1: Download Windows Server

> Download [Windows Server ISO 64 bit](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022)

<br>

## Step 2: Create new VM

> Launch Oracle VBM and select "New"
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 120118.png">
>
> Follow along with below images on completing the VM setup
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 121303.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 121942.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 124057.png">

<br>

## Step 3: Network Settings

> Select the Windows Server VM's settings and then network
>
> In Network settings configure the following
> 
> <img src="assets/WS&AD/Screenshot 2024-12-24 125742.png">

<br>

## Step 4: Installing Windows Server on VM

> Launch the Windows Server VM
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 130542.png">
>
> Once VM launches, follow through the installation process
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 130958.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 131248.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 131321.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 131335.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 131356.png">
>
> Once the installation is complete the system will reboot then prompt for the creation of a local Administrator account

<br>

## Step 5: Configuring Windows Server

> Login to Windows Server
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 132559.png">
>
> Open Network & Internet Settings
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 132651.png">
>
> Follow below images to configure Window Server IPv4 Network settings
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 132819.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 132846.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 132909.png">
>
> Assign a Static IP, Subnet, and Gateway ("LAN" IP Address from pfSense VM). The Preferred DNS server will be the IP Address of the Windows Server machine, then another known DNS server (ex. Google's DNS Server)
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 132948.png">
>
> Next rename Windows Server and restart
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 135432.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 135440.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 135457.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 135504.png">

<br>

## Step 6: Installing Active Directory

> After restart and logging in, open Server Manager then Add roles and features
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 140046.png">
>
> Follow images below to install Active Directory
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 140135.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 140144.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 140221.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 140457.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 140237.png">
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 140444.png">
>
> After install open the Warning Flag to promote the server as a domain controller
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 140853.png">
>
> Add a new forest and name it
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 141035.png">
> 
> Leave default configuration, create password, and restart after the domain is configured.
>
> <img src="assets/WS&AD/Screenshot 2024-12-24 141340.png">

<br>

## Step 7: Configure AD

> Download [BadBlood](https://github.com/davidprowe/BadBlood?tab=readme-ov-file) script on the Windows Server VM to populate AD with misconfiguration to analyze and remediate
>
> Launch Powershell as Administrator
>
> Change directory to the Badblood folder
>
> Launch Invoke-BadBlood.ps1 file
>
> Script will automate AD configuration with new accounts

<br>

# _Windows Server Setup is complete_

<br>

[Back To Project's Homepage](https://brismit25.github.io/Home-SOC-Lab-Setup/)
