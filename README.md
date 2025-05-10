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

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 1:</b> Log in to the osTicket admin panel using the credentials you created during installation. Navigate to the dashboard to begin configuration.</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 2:</b> Delete the <code>/setup</code> directory from <code>C:\inetpub\wwwroot\osTicket</code>. This is a critical security step after installation is complete.</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 3:</b> Locate the <code>ost-config.php</code> file in the <code>include</code> folder. Right-click the file, go to Properties, and set it to read-only to prevent accidental changes.</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 4:</b> Go to <b>Admin Panel > Emails > System Emails</b> and configure your primary support email address (e.g., support@yourdomain.com). This email will send/receive ticket updates.</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 5:</b> Navigate to <b>Admin Panel > Staff > Departments</b> and create key departments like IT Support, Billing, or Customer Service to help route incoming tickets appropriately.</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 6:</b> Go to <b>Admin Panel > Manage > Help Topics</b> and create topics such as “Password Reset” or “Order Status” to streamline ticket categorization for users submitting tickets.</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 7:</b> Add your staff by going to <b>Admin Panel > Staff > Agents</b>. Create agent accounts, assign them to departments, and define access roles (e.g., Admin, Staff).</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Step Image"/>
</p>
<p><b>Step 8:</b> Under <b>Admin Panel > Settings > Tickets</b>, configure ticket options like auto-responses, SLA settings, ticket priorities, and visibility rules to optimize your workflow.</p>
<br />
