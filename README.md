<p align="center">
<img src="https://imgur.com/bGOgZG9.png" alt="msAzure logo">
</p>

<h1>Active Directory Configuration Within Azure</h1>
This tutorial outlines the configuration of Active Directory in Microsoft Azure. <br />


<h2>Environments and Technologies Used</h2>

- Azure portal
- Remote Desktop
- Command Prompt
  

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>
- Resource Group in Azure
- Remote Desktop Client

  

<h2>Active Directory</h2>

<p>
<img src="https://imgur.com/uZVI32a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Azure portal, inside your selected Resource Group, create the Domain Controller's Virtual Machine, a Windows Server, name it. This tutorial will display a controller named "DC-1". A second Virtual Machine is created and named Client-1. Connectivity must be ensured between the two Virtual Machines by doing a perpetual ping. Login to the DC-1 Controller machines using Remote Desktop and enable ICMPv4 You on the local firewall. Client-1 show display a successful ping.
</p
<br />

<p>
<img src="https://imgur.com/5XIc0US.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Login to DC-1 and install Active Directory Domain Services from the web. Setup a new forest, you can use mydomain.com for example. 
</p>
<br />

<img src="https://imgur.com/mucef8L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Restart and login back in using mydomain.com/labuser, then go on to create both an Admin and User Account inside the Active Directory. Create an organizational unit called "Employees" and another called "Admins". Create an employee. For example: Jane Doe. Jane Doe can be added as an Admin. Jane must be added to the Domain Admins Security Group. To observe the change log out/close the Remote Desktop, log back in as mydomain.com\jane_admin
</p>
<br />


