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
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/8745c905-29b0-4396-a085-6f9fbb707c69" />
</p>
<p>
Using this link, you can log in as an Admin: http://localhost/osTicket/scp/login.php

Using this link, you can submit a ticket as an end user: http://localhost/osTicket 
</p>
<br />

<p>
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/be9349d1-0c61-4872-a83c-e1a964a09156" />
</p>
<p>
Configure Roles for grouping permissions

In the admin panel, select agents, then roles
Add a new role called Supreme admin with all permissions 
</p>
<br />

<p>
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/99975a6f-f341-4e73-90ae-8a94a9503520" />
</p>
<p>
Configure Departments Ticket Visibility

In the admin panel, select departments > add a new department > and select Top-Level department >

name SysAdmins, and Create

Delete the Maintenance Department (not archive, for the tutorial)
</p>
<br />

<p>
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/ff00b5ec-c363-4f2e-8cbe-7c7275359e88" />
</p>
<p>
Configure Teams

In the admin panel, select Agents > Teams > and add a new team called Online banking 
</p>
<br />

<p>
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/242a2a8f-d74f-4a41-99d4-92eba2ea0611" />
</p>
<p>
To allow anyone to create a ticket without an account, go to settings > users > uncheck registration required 
</p>
<br />

<p>
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/865ce292-39a0-4e0e-bd6d-a2656f510cd3" />
</p>
<p>
Configure two Agents (Workers) by filling in name, email, and username, then go to > Admin Panel > Agents > add new 
Set a password > uncheck “Send the agent a password reset email,” and set the password

</p>
<br />

<p>
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/bdb9feae-8eb5-46b6-9eca-3dc1c20ee120" />
</p>
<p>
Assign the first agent to the SysAdmin with supreme admin, add them to the online banking team, and assign the second agent to support with view only
</p>
<br />

<p>
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/7cabc0a3-6079-4909-b2ce-a634ab6bd528" />
</p>
<p>
Open the Agent Panel, Users, and select Add user
(You will only need to put an email and a name for this tutorial)
</p>
<br />

<p>
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/c9063aed-fea8-4801-b4cc-637f6bde8316" />
</p>
<p>
Configure SLA
Open the Admin Panel, manage, then SLA

Sev-A (Grace Period: 1 hour, Schedule: 24/7) >
Sev-B (Grace Period: 4 hours, Schedule: 24/7) >
Sev-C (Grace Period: 8 hours, Business Hours)
</p>
<br />

<p>
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/be1b61da-6819-4952-ba98-31072187cb88" />
</p>
<p>
Configure Help Topic (For when users create a ticket)
Open Admin Panel, Manage, Help Topic, then select Add New Help Topic
Examples used in the tutorial
Business Critical Outage (Report Problem)
Personal Computer Issues (Report Problem)
Equipment Request (General Inquiry)
Password Reset (Report Problem)
Other (General Inquiry)  
</p>
<br />
