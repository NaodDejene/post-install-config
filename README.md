<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
<p>This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.</p>

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Internet Information Services (IIS)</li>
</ul>

<h2>Operating Systems Used</h2>
<ul>
  <li>Windows 10 (21H2)</li>
</ul>

<h2>Post-Install Configuration Objectives</h2>
<ul>
  <li>Delete the setup directory for security</li>
  <li>Set configuration file to read-only</li>
  <li>Configure support email accounts</li>
  <li>Create departments and help topics</li>
  <li>Add agents and assign roles</li>
  <li>Customize ticket settings and workflows</li>
  <li>Ensure PHP extensions and permissions are correctly set</li>
  <li>Prepare osTicket for real-time use</li>
</ul>

<h2>Configuration Steps</h2>

<!-- Step 1 -->
<p><img src="https://i.imgur.com/wN7VM5W.png" height="80%" width="80%" alt="Step 1 Image 1"/></p>
<p><img src="https://i.imgur.com/6QwSl3H.png" height="80%" width="80%" alt="Step 1 Image 2"/></p>
<p><b>Step 1:</b> Configure Roles - for grouping permissions<br/>
Navigate to: Admin Panel > Agents > Roles<br/>
Create Role: <i>Supreme Admin</i></p>
<br/>

<!-- Step 2 -->
<p><img src="https://i.imgur.com/m2hcKbx.png" height="80%" width="80%" alt="Step 2 Image 1"/></p>
<p><img src="https://i.imgur.com/p0WrJwj.png" height="80%" width="80%" alt="Step 2 Image 2"/></p>
<p><b>Step 2:</b> Configure Departments (Ticket Visibility)<br/>
Navigate to: Admin Panel > Agents > Departments<br/>
Create Department: <i>SysAdmins</i></p>
<br/>

<!-- Step 3 -->
<p><img src="https://i.imgur.com/aowZ2Ab.png" height="80%" width="80%" alt="Step 3 Image 1"/></p>
<p><img src="https://i.imgur.com/RsNAeDB.png" height="80%" width="80%" alt="Step 3 Image 2"/></p>
<p><img src="https://i.imgur.com/Y8hTaCj.png" height="80%" width="80%" alt="Step 3 Image 3"/></p>
<p><b>Step 3:</b> Configure Teams<br/>
Navigate to: Admin Panel > Agents > Teams<br/>
Team Name: <i>Online Banking</i> (pull agents from different departments)</p>
<br/>

<!-- Step 4 -->
<p><img src="https://i.imgur.com/Or3ixIA.png" height="80%" width="80%" alt="Step 4 Image 1"/></p>
<p><b>Step 4:</b> Allow anyone to create tickets<br/>
Navigate to: Admin Panel > Settings > User Settings<br/>
Uncheck: <i>Unregistered users can create tickets</i><br/>
Check: <i>Registration Required – Require login to create tickets</i></p>
<br/>

<!-- Step 5 -->
<p><img src="https://i.imgur.com/Z4M6NYQ.png" height="80%" width="80%" alt="Step 5 Image 1"/></p>
<p><img src="https://i.imgur.com/cE55C5R.png" height="80%" width="80%" alt="Step 5 Image 2"/></p>
<p><img src="https://i.imgur.com/pMTlPZa.png" height="80%" width="80%" alt="Step 5 Image 3"/></p>
<p><b>Step 5:</b> Configure Agents (Workers)<br/>
Navigate to: Admin Panel > Agents > Add New<br/>
Create Agent: <i>Jane</i> (Department: SysAdmins)<br/>
Create Agent: <i>John</i> (Department: Support)</p>
<br/>

<!-- Step 6 -->
<p><img src="https://i.imgur.com/ppICdZT.png" height="80%" width="80%" alt="Step 6 Image 1"/></p>
<p><img src="https://i.imgur.com/9Nk1a0k.png" height="80%" width="80%" alt="Step 6 Image 2"/></p>
<p><img src="https://i.imgur.com/wYeDWXs.png" height="80%" width="80%" alt="Step 6 Image 3"/></p>
<p><b>Step 6:</b> Configure Users (Customers)<br/>
Navigate to: Agent Panel > Users > Add New<br/>
Create User: <i>Karen</i><br/>
Create User: <i>Ken</i></p>
<br/>

<!-- Step 7 -->
<p><img src="https://i.imgur.com/NrbpyMT.png" height="80%" width="80%" alt="Step 7 Image 1"/></p>
<p><img src="https://i.imgur.com/GiTJePD.png" height="80%" width="80%" alt="Step 7 Image 2"/></p>
<p><b>Step 7:</b> Configure SLA<br/>
Navigate to: Admin Panel > Manage > SLA<br/>
Define SLA Plans:<br/>
- Sev-A: 1 hour, 24/7<br/>
- Sev-B: 4 hours, 24/7<br/>
- Sev-C: 8 hours, Business Hours</p>
<br/>

<!-- Step 8 -->
<p><img src="https://i.imgur.com/fBVGeaW.png" height="80%" width="80%" alt="Step 8 Image 1"/></p>
<p><img src="https://i.imgur.com/0EyrNAb.png" height="80%" width="80%" alt="Step 8 Image 2"/></p>
<p><img src="https://i.imgur.com/lNUukbD.png" height="80%" width="80%" alt="Step 8 Image 3"/></p>
<p><b>Step 8:</b> Configure Help Topics (For when users create a ticket)<br/>
Navigate to: Admin Panel > Manage > Help Topics<br/>
Create the following help topics:<br/>
- Business Critical Outage<br/>
- Personal Computer Issues<br/>
- Equipment Request<br/>
- Password Reset<br/>
- Other</p>
<br/>

