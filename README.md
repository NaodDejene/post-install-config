<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Video Demonstration</h2>
- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>
- Microsoft Azure (Virtual Machines/Compute)  
- Remote Desktop  
- Internet Information Services (IIS)

<h2>Operating Systems Used</h2>
- Windows 10 (21H2)

<h2>Post-Install Configuration Objectives</h2>
- Delete the setup directory for security  
- Set configuration file to read-only  
- Configure support email accounts  
- Create departments and help topics  
- Add agents and assign roles  
- Customize ticket settings and workflows  
- Ensure PHP extensions and permissions are correctly set  
- Prepare osTicket for real-time use  

<h2>Configuration Steps</h2>

<!-- Step 1 -->
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 1:</b> Configure Roles (for grouping permissions)<br/>
Admin Panel → Agents → Roles<br/>
Create Role: Supreme Admin
</p>
<br />

<!-- Step 2 -->
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 2:</b> Configure Departments (Ticket Visibility)<br/>
Admin Panel → Agents → Departments<br/>
Create Department: SysAdmins
</p>
<br />

<!-- Step 3 -->
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 3:</b> Configure Teams<br/>
Admin Panel → Agents → Teams<br/>
Team Name: Online Banking (Pull Agents from different Departments)
</p>
<br />

<!-- Step 4 -->
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 4:</b> Allow anyone to create tickets<br/>
Admin Panel → Settings → User Settings<br/>
UNCHECK: Unregistered users can create tickets<br/>
CHECK: Registration Required – Require login to create tickets
</p>
<br />

<!-- Step 5 -->
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 5:</b> Configure Agents (Workers)<br/>
Admin Panel → Agents → Add New<br/>
Create Agent: Jane (Dept: SysAdmins)<br/>
Create Agent: John (Dept: Support)
</p>
<br />

<!-- Step 6 -->
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 6:</b> Configure Users (Customers)<br/>
Agent Panel → Users → Add New<br/>
Create User: Karen<br/>
Create User: Ken
</p>
<br />

<!-- Step 7 -->
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 7:</b> Configure SLA<br/>
Admin Panel → Manage → SLA<br/>
Sev-A: 1 hour, 24/7<br/>
Sev-B: 4 hours, 24/7<br/>
Sev-C: 8 hours, Business Hours
</p>
<br />

<!-- Step 8 -->
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%"

