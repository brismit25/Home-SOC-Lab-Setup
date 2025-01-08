---
layout: default
---

# Kali Linux Setup

## Step 1: Download Kali Linux

> Download [Kali Linux 64 bit](https://www.kali.org/get-kali/#kali-platforms)

<br>

## Step 2: Create new VM

> Launch Oracle VBM and select "New"
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 073314.png">
>
> Follow along with below images on completing the VM setup
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 073431.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 073755.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 074039.png">

<br>

## Step 3: Network Settings

> Select the Kali Linux VM's settings and then network
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 074220.png">
>
> In Network settings configure the following
> 
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 074257.png">

<br>

## Step 4: Installing Kali Linux on VM

> Launch the Kali Linux VM
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 074506.png">
>
> Once VM launches, follow through the Kali Linux Installation process
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 074607.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 074704.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 074734.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 074756.png">
>
> Linux will prompt to configure Network Settings due to not have network connectivity
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 075211.png">
>
> Configure a static IP address with subnet mask
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 075241.png">
>
> Gateway will be the _LAN_ IP Address from pfSense VM
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 075630.png">
> 
> _Name Servers_ will be the IP address of your Windows Server, and a backup known DNS server like Google
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 075947.png">
>
> Then proceed with the final installation options below
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 080637.png">
>
> Input the domain name that was created with the Active Directory setup 
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 080926.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 081037.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 081459.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 081622.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 082330.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 082459.png">
>
> Install GRUB boot loader
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 083249.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 083317.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 083736.png">
>
> <img src="assets/KaliLinSetup/Screenshot 2025-01-07 084226.png">

<br>

# _Kali Linus Setup is complete_

<br>

[Back To Project's Homepage](https://brismit25.github.io/Home-SOC-Lab-Setup/)
