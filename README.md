<p align="center">
<img src="https://i.imgur.com/IKrl3hC.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Network File Shares and Permissions</h1>
This tutorial we will be sharing out files and folders over the network and allow different people and groups with different levels of access.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (22H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create file shares with variouis permissions
- Attempt to access file shares as a normal user
- Create an "ACCOUNTANTS" Security Group, assign permissions, and test access

<h2>Deployment and Configuration Steps</h2>

<p>
 We use File Shares when we want to share out files/folders to a large group of people. Some people might have Read-only access, while some might have both Read/Write, and we might have files where no people will have access to except only to a few select people. 
</p>

<p>
 First we are going to connect to DC-1 from our last lab and login as John Doe (admin). From Active Directory Users and Computers, we are going to find a normal user (non-administrative) and connect to Client-1 with the login of that normal user. For this we will use: Cato Hux. 
 <br/>
 <br/>
 Then in DC-1's C:\ drive, we will create folders and set the following permissions for the "Domain Users" group:
 <br/>
 Folder: "read-access", Group: "Domain Users", Permission: "Read"
 <br/>
 Folder: "write-access", Group: "Domain Users", Permission: "Read/Write"
 <br/>
 Folder: "no-access", Group: "Domain Admins", Permission: "Read/Write"
 <br/>
 Folder" "accounting", (Skip Group and Permission for now)
</p>
<p>
<img src="https://i.imgur.com/IZO0FY6.png" height="80%" width="80%" alt="xxx"/>
 <br/>
 <img src="https://i.imgur.com/sbMt4uZ.png" height="80%" width="80%" alt="xxx"/>
  <br/>
 <img src="https://i.imgur.com/8z1UA1k.png" height="80%" width="80%" alt="xxx"/>
  <br/>
 <img src="https://i.imgur.com/5FjjtKx.png" height="80%" width="80%" alt="xxx"/>
 <p/>
<br/>
<br/>
<br/>
 
