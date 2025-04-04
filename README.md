<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the how to configure osTicket and go over a few terms we might see in the work force.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>osTicket Admin Panel Configuration Lab</h2>

Now that we have installed osTicket and accessed the admin panel, let’s configure it.

If you haven't installed osTicket yet, please refer to my [osTicket installation lab](https://github.com/ashotshe/osticket-prereqs/blob/main/README.md).

1. Log into the Admin Panel
Log in with your admin account first. Once logged in, click on the Admin Panel. You will notice many additional options appear.

2. Create Roles and Groups
We will begin by creating roles that define different access levels for different groups. Groups are used to assign permissions to different people.

Create a Role:

Go to Admin Panel → Manage → Roles.

Create a new role called System Admins and give them all permissions.

Create a Group:

Go to Admin Panel → Manage → Groups.

Create a group called System Admins and assign the System Admins role to this group.

3. Create a Department
Next, let's create a department for system admins.

Go to Admin Panel → Manage → Departments.

Create a new department called Sys Admins.

4. Create a Team
Teams allow you to pull agents from different departments into one team.

Go to Admin Panel → Manage → Teams.

Create a team called Shield.

5. Adjust Ticket Registration Settings
For this lab, we want everyone to be able to register tickets.

Go to Admin Panel → Settings → Users.

Make sure the box labeled "Allow users to register tickets" is unchecked.

6. Create Agents
Now we will create a few agents (workers) to assign roles and teams.

Go to Admin Panel → Manage → Agents.

Click on Agents and add a new agent.

Agent 1:

Name: Gwen Stacy

Role: Superior Admin (full access)

Team: Shield

Agent 2:

Name: Harry Osborn

Role: Support (view access only)

Team: Shield

Make sure to record the email addresses for these agents, as they will be required for login.

7. Create a User
Now, let's create a user for ticket submission.

Go to the top-right corner and click on Agent Panel.

Navigate to Users and click Add New User.

Create a user with the name Norman Osborn (for this lab, we’ll create just one user).

8. Configure SLA (Service Level Agreements)
SLAs are used to notify agents how quickly a ticket should be handled.

Go to Admin Panel → Manage → SLA.

Create the following 3 SLAs:

SEV-A: Critical – needs immediate attention

SEV-B: Medium priority

SEV-C: Low priority

9. Create Help Topics
Help Topics guide users when they create tickets, directing them toward the correct category.

Go to Admin Panel → Manage → Help Topics.

Create the following Help Topics:

Personal Computer (with the sub-topic Report a Problem)

Equipment Request (with the sub-topic General Inquiry)

Conclusion
This lab is a prerequisite for the next lab, where we will practice using the ticketing system. Follow these steps to set up your admin panel, roles, groups, agents, and SLAs in preparation for the next steps
