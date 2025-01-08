---
layout: default
---

# Windows Sysmon Setup

<br>

## Step 1: Download Windows Sysmon Software

> On the Windows Server and Windows 11 VM, download [Windows Sysmon](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)
> 
> Also download [Sysmon Configuration File](https://github.com/olafhartong/sysmon-modular/blob/master/sysmonconfig.xml)
>
> Save the Sysmon Configuration File into the Windows Sysmon Folder

<br>

## Step 2: Install Sysmon

> Launch Powershell in Administrator mode
>
> Change directory to the Windows Sysmon Folder
>
> Install Sysmon with command **_sysmon.exe -accepteula -i YOURFILE.xml_**
> 
> <img src="assets/WinSysmon/Screenshot 2025-01-02 100251.png">

<br>

# _Windows Sysmon Setup is complete_

<br>

[Back To Project's Homepage](https://brismit25.github.io/Home-SOC-Lab-Setup/)
