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

- Acknowledge Agent vs Admin accounts
- Configure roles, departments, and teams
- Choose who can create a ticket
- Configure SLA 
- Create Help Topics (for when users create a ticket)

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/G2N0TfY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/M1f7CQm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
  We begin by adding a "supreme admin" role that has full permissions. 
Configure Roles (for grouping permissions)
Admin Panel -> Agents -> Roles. We will do the same process for adding departments and teams. This can only be done from an administrator account.

</p>
<br />

<p>
<img src="https://i.imgur.com/kZa1Tx2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigating to the user settings. Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
Registration Required: Require registration and login to create tickets. We have selected to require registration and login to create tickets. We do not want outside parties to create tickets for our employees.
</p>
<br />

<p>
<img src="https://i.imgur.com/7Ot07Se.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate to Configure SLA
Admin Panel -> Manage -> SLA. We will create 3 different SLAs based on the severity of the issue.
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)

</p>
<br />

<p>
<img src="https://i.imgur.com/spg2YyX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure Help Topics (For when users create a ticket)
Admin Panel -> Manage -> Help Topics
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other


</p>
<br />
