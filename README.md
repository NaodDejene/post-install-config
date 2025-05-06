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

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Item 1 secure your installation
- Item 2 log in and set up agents and departments
- Item 3  set up email and help topics


<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Connect to your Azure VM via remote desktop and then navigate to C:\inetpub\wwwroot\upload and delete or rename the setup folder and then set ost-config.php to read only" Right click > properties>security > Remove "write" permissions and then secure your enviorment after installation. </p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to http://<your-VM-IP>/upload/scp in your browser. Log in using the admin credentials created during setup . And in the Admin panel : create departments, create roles and assign permission and add agents and assign then roles or departments.

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to Emails> Add email addresses, configure SMTP/IMAP for sending and recieving, set up a windows tast schedular job to run cron.php every 5 - 10 minutes, go to manage> Help topics to create option like "passwpord Reset" or " Billing Question". r</p>
<br />
