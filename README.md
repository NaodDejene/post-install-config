<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

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
  <img src="https://i.imgur.com/wN7VM5W.png" height="80%" width="80%" alt="Step 1 Image 1"/>
</p>
<p>
  <img src="https://i.imgur.com/6QwSl3H.png" height="80%" width="80%" alt="Step 1 Image 2"/>
</p>
<p><b>Step 1:</b> Configure Roles -for grouping permission <br/>
Go to Admin Panel → Agents → Roles<br/>
Create Role: Supreme Admin
</p>
<br />

<!-- Step 2 -->
<p>
  <img src="https://i.imgur.com/m2hcKbx.png" height="80%" width="80%" alt="Step 2 Image 1"/>
</p>
<p>
  <img src="https://i.imgur.com/p0WrJwj.png" height="80%" width="80%" alt="Step 2 Image 2"/>
</p>
<p><b>Step 2:</b> Configure Departments (Ticket Visibility)<br/>
Go to Admin Panel → Agents → Departments<br/>
Create Department: SysAdmins
</p>
<br />

<!-- Step 3 -->
<p>
  <img src="https://i.imgur.com/aowZ2Ab.png" height="80%" width="80%" alt="Step 3 Image 1"/>
</p>
<p>
  <img src="https://i.imgur.com/RsNAeDB.png" height="80%" width="80%" alt="Step 3 Image 2"/>
</p>
<p>
  <img src="https://i.imgur.com/Y8hTaCj.png" height="80%" width="80%" alt="Step 3 Image 3"/>
</p>
<p><b>Step 3:</b> Configure Teams<br/>
Go to the Admin Panel and then go to Agents → Teams<br/>
Team Name: Online Banking (Pull Agents from different Departments)
</p>
<br />

<!-- Step 4 -->
<p>
  <img src="https://i.imgur.com/Or3ixIA.png" height="80%" width="80%" alt="Step 4 Image 1"/>
</p>
<p><b>Step 4:</b> Allow anyone to create tickets<br/>
Go to the Admin Panel and then  Settings and then  User Settings<br/>
uncheck Unregistered users can create tickets<br/>
and make sure to chec Registration Required – Require login to create tickets
</p>
<br />

<!-- Step 5 -->
<p>
  <img src="https://i.imgur.com/Z4M6NYQ.png" height="80%" width="80%" alt="Step 5 Image 1"/>
</p>
<p>
  <img src="https://i.imgur.com/cE55C5R.png" height="80%" width="80%" alt="Step 5 Image 2"/>
</p>
<p>
  <img src="https://i.imgur.com/pMTlPZa.png" height="80%" width="80%" alt="Step 5 Image 3"/>
</p>
<p><b>Step 5:</b> Configure Agents (Workers)<br/>
Go to Admin Panel → and then Agents → Add New<br/>
Create Agent: Jane (Dept: SysAdmins)<br/>
Create Agent: John (Dept: Support)
</p>
<br />

<!-- Step 6 -->
<p>
  <img src="https://i.imgur.com/ppICdZT.png" height="80%" width="80%" alt="Step 6 Image 1"/>
</p>
<p>
  <img src="https://i.imgur.com/9Nk1a0k.png" height="80%" width="80%" alt="Step 6 Image 2"/>
</p>
<p>
  <img src="https://i.imgur.com/wYeDWXs.png" height="80%" width="80%" alt="Step 6 Image 3"/>
</p>
<p><b>Step 6:</b> Configure Users (Customers)<br/>
Go to Agent Panel → Users → Add New<br/>
Create User: Karen<br/>
Create User: Ken
</p>
<br />

<!-- Step 7 -->
<p>
  <img src="https://i.imgur.com/NrbpyMT.png" height="80%" width="80%" alt="Step 7 Image 1"/>
</p>
<p>
  <img src="https://i.imgur.com/GiTJePD.png" height="80%" width="80%" alt="Step 7 Image 2"/>
</p>
<p><b>Step 7:</b> Configure SLA<br/>
Go to Admin Panel → Manage → SLA<br/>
Sev-A: 1 hour, 24/7<br/>
Sev-B: 4 hours, 24/7<br/>
Sev-C: 8 hours, Business Hours
</p>
<br />

<!-- Step 8 -->
<p>
  <img src="https://i.imgur.com/fBVGeaW.png" height="80%" width="80%" alt="Step 8 Image 1"/>
</p>
<p>
  <img src="https://i.imgur.com/0EyrNAb.png" height="80%" width="80%" alt="Step 8 Image 2"/>
</p>
<p>
  <img src="https://i.imgur.com/lNUukbD.png" height="80%" width="80%" alt="Step 8 Image 3"/>
</p>
<p><b>Step 8:</b> Configure Help Topics (For when users create a ticket)<br/>
Go to Admin Panel → Manage → Help Topics<br/>
Create the following help topics:<br/>
- Business Critical Outage<br/>
- Personal Computer Issues<br/>
- Equipment Request<br/>
- Password Reset<br/>
- Other
</p>
<br />
