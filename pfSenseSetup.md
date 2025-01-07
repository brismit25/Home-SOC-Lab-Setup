---
layout: default
---

# Step 1: Download pfSense

> Download [pfSense](https://www.pfsense.org/download/) (AMD64 ISO IPMI/Virtual Machine)

# Step 2: Create New VM for pfSense

> Launch Oracle VBM and select "New"
> 
> <img src="assets/pfSense/Creating New VM.png">
>
> Follow along with below images on completing the VM setup
>
> <img src="assets/pfSense/pfSense Config 1.png">
>
> <img src="assets/pfSense/pfSense Config 2.png">
>
> <img src="assets/pfSense/pfSense Config 3.png">

# Step 3: Network Settings

> Select the pfSense VM's settings and then network
>
> In Network settings configure the following
>
> <img src="assets/pfSense/Screenshot 2025-01-07 133847.png">
>
> <img src="assets/pfSense/pfSense Network 3.png">
>
> <img src="assets/pfSense/pfSense Network 4.png">
>
> Make sure to document the MAC Address for each Adapter for later reference

# Step 4: Installing pfSense on VM

> Launch the pfSense VM
>
> <img src="assets/pfSense/Launching pfSense.png">
>
> Accept Copyright and Trademark Notice
>
> <img src="assets/pfSense/Install pfSense 1.png">
> 
> Proceed with pfSense installation
>
> <img src="assets/pfSense/Install pfSense 2.png">
>
> <img src="assets/pfSense/Install pfSense 3.png">
> 
> Verify MAC Addresses
>
> <img src="assets/pfSense/Install pfSense 4.png">
> 
> WAN Interface will be left as DHCP
>
> <img src="assets/pfSense/Install pfSense 5.png">
> 
> LAN Interface will be the "GREEN" Network Adapter
>
> <img src="assets/pfSense/Install pfSense 8.png">
> 
> Assign a Static IP for the LAN Interface
>
> <img src="assets/pfSense/Install pfSense 9.png">
> 
> Once install completes reboot the VM
>
> <img src="assets/pfSense/Install pfSense 6.png">
>
> <img src="assets/pfSense/Install pfSense 7.png">
>
> If VM gets stuck in installation reboot cycle go into the VM's setting and Storage, then remove the Controller: IDE
>
> <img src="assets/pfSense/Picture1.png">

# Step 5: pfSense Network Configuration

> In pfSense main menu select Option 1
>
> <img src="assets/pfSense/Screenshot 2024-12-24 103323 (option 1).png">
>
> Verify WAN/LAN is set to the correct MAC Addresses, then assign DMZ Adapter to Optional 1 Interface
>
> <img src="assets/pfSense/Screenshot 2024-12-24 104518.png">
>
> <img src="assets/pfSense/Screenshot 2024-12-24 104639.png">
>
> <img src="assets/pfSense/Screenshot 2024-12-24 104730.png">
>
> Then confirm the choices
>
> <img src="assets/pfSense/Screenshot 2024-12-24 104916.png">
>
> Next, configure LAN IP and Subnet (leave gateway as none)
>
> <img src="assets/pfSense/Screenshot 2024-12-24 105242.png">
>
> <img src="assets/pfSense/Screenshot 2024-12-24 105331.png">
>
> <img src="assets/pfSense/Screenshot 2024-12-24 105454.png">

# _pfSense Setup is complete_

<br>

[Back To Project's Homepage](https://brismit25.github.io/Home-SOC-Lab-Setup/)
