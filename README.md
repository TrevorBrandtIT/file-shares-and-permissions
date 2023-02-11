<p align="center">
<img src="https://i.imgur.com/AeiqMDZ.png" alt="File Share Graphic"/>
</p>

<h1>Building Intuition with DNS</h1>
This tutorial covers experimenting with and gaining a better understanding of DNS.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Creating sample file shares and permissions.
- Attempting to access file shares as a normal user.
- Creating, assigning permissions to, and testing access of an Accountants Security Group.


<h2>Deployment and Configuration Steps</h2>

<p>
Welcome back to the final part of my Active Directory Tutorials. I'll be assuming that you've just finished the previous tutorial. If not, go back through the previous two tutorials to catch up.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First things first, go ahead and log into DC-1 as Jane Doe. We'll be logging into Client-1 as one of the Users we created earlier with the PowerShell script. Remember, the password for all of those accounts is "Password1". Once logged in as one of those users, go back to DC-1. Create 4 folders on the C: drive, name them "read_access", "write_access", "no_access", and "accounting". From here, right click each folder and share the folder with:
<ol type="1">
   <li>Folder: “read_access”, Group: “Domain Users”, Permission: “Read”</li>
   <li>Folder: “write_access”,  Group: “Domain Users”, Permissions: “Read/Write”</li>
   <li>Folder: “no_access”,  Group: “Domain Admins”, Permissions: “Read/Write”</li>
</ol>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /> 

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
That concludes my series of tutorials in Active Directory. I hope you enjoyed!
</p>
<br />
