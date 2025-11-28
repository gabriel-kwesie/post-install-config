<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Teams
- Configure Agents
- Configure SLA
- Configure Help Topic

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Using this link, you can log in as an Admin: http://localhost/osTicket/scp/login.php

Using this link, you can submit a ticket as an end user: http://localhost/osTicket 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure Roles for grouping permissions

In the admin panel, select agents, then roles
Add a new role called Supreme admin with all permissions 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure Departments Ticket Visibility

In the admin panel, select departments > add a new department > and select Top-Level department >

name SysAdmins, and Create

Delete the Maintenance Department (not archive, for the tutorial)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure Teams

In the admin panel, select Agents > Teams > and add a new team called Online banking 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To allow anyone to create a ticket without an account, go to settings > users > uncheck registration required 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure two Agents (Workers) by filling in name, email, and username, then go to > Admin Panel > Agents > add new 
Set a password > uncheck “Send the agent a password reset email,” and set the password

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Assign the first agent to the SysAdmin with supreme admin, add them to the online banking team, and assign the second agent to support with view only
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open the Agent Panel, Users, and select Add user
(You will only need to put an email and a name for this tutorial)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure SLA
Open the Admin Panel, manage, then SLA

Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure Help Topic (For when users create a ticket)
Open Admin Panel, Manage, Help Topic, then select Add New Help Topic
Examples used in Lab
Business Critical Outage (Report Problem)
Personal Computer Issues (Report Problem)
Equipment Request (General Inquiry)
Password Reset (Report Problem)
Other (General Inquiry)  
</p>
<br />
