<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1 VM creation
- Step 2 Connectivity
- Step 3 Installing Active Directory
- Step 4 Setting up Active Directory
- Step 5 Adding Users and logging into client vm

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/gbQtvZp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The first step in this lab was to create the virtual machines, one being for the domain controller and the other for the client. 
</p>
<br />

<p>
<img src="https://i.imgur.com/8ei5MdB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After creating the vm for both I checked for connectivity between them by logging into one then pinging the other.
</p>
<br />

<p>
<img src="https://i.imgur.com/VZ8MOVO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I then started the process to install Active Directory. 
</p>
<br />

<p>
<img src="https://i.imgur.com/KFaPmSg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once the installation was complete I went into Active Directory and created two organizational units, one for admins and the other for employees.  
</p>
<br />

<p>
<img src="https://i.imgur.com/FdCUmGh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Then, I began to create a account to be an admin inside of Active Directory.  
</p>
<br />

<p>
<img src="https://i.imgur.com/l361Bre.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 After creating the account I needed to then join the clients vm to the domain controllers vm. 
</p>
<br />

<p>
<img src="https://i.imgur.com/nMuQxi4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 To complete the lab I then used powershell to create a plethora of users. The users being created were made to fall into the employees organizational unit, and I then logged into the clients vm with one of the random accounts. 
</p>
<br />
