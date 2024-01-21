# Active Directory-Bulk User Creation w/PowerShell

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo) 📺

<h2>Description</h2>


This Project that I set up consists of creating Virtual Machines with Oracle Virtual Box and building a Home Lab running Active Directory Domain Services on Windows Server. The goal of this lab is to simulate a work environment by assigning IP addresses to Internal NICs, Installing RAS and NAT on a domain controller to allow clients to access internal network and outward facing internet, Setting up a DHCP sever with a set scope on a domain controller to maintain DNS and DHCP services, and Using PowerShell scripts to create and manage a bulk of users in Active Directory. Below is a diagram that gives you a good idea of the order of events in this Lab.
<img src="https://imgur.com/jGWGGkY.png" height="50%" width="70%" alt="Disk Sanitization Steps"/>
<br />

<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b>
- <b>Active Directory Users and Computers</b>
- <b>DHCP Server</b>
- <b>Oracle VM VirtualBox</b>
<h2>Environments Used </h2>

- <b>Windows Server 2019</b> 
- <b>
  <b>Windows 10</b> (21H2)
<h2>Lab Walk-Through:</h2>

<p align="center">
Set up your Homelab: 
<br>First download Orcale VM, Windows 10 ISO,Server 2019 ISO, and PowerShell Script (download in repo files): <br/>
  <br>https://www.virtualbox.org/wiki/Downloads<br/>
  <br>https://www.microsoft.com/en-us/software-download/windows10<br/>
  <br>https://www.microsoft.com/en-us/evalcenter/download-windows-server-2019<br/>
  <br><br/>
<br />
Install Active Directory Domain Services on the Windows Server VM using Server Manager:  <br/>
<img src="https://i.imgur.com/TQvSZUs.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create the Domain: <br/>
<img src="https://i.imgur.com/2EsUWQ1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install RAS and NAT on domain controller:  <br/>
<img src="https://i.imgur.com/K38pceO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<img src="https://i.imgur.com/4Ya3Ju6.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>  
<br />
<br />
Set up a DHCP sever:  <br/>
<img src="https://i.imgur.com/DqRHvLb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<img src="https://i.imgur.com/M4rrZFi.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
  <br />
<br />
Open "CREATE_USERS" Script file in PowerShell ISE:  <br/>
<img src="https://i.imgur.com/DMaLLvi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Run The Script and create the users:  <br/>
<img src="https://i.imgur.com/8uLdkEg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
Test to see if one of the New User's can log onto a windows 10 client with their creds:  <br/>
<img src="https://i.imgur.com/NYCWFp1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
Finally ping to the internet to see if you have access to the internal network and outward facing network:  <br/>

<img src="https://i.imgur.com/nQ5XdXp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
