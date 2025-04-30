<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This demonstration outlines the next steps to setting up an osTicket environment after it is installed.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: osTicket Post-Install Configuration](https://youtu.be/p4DydgvwAOU)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket Control Panel

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Overview of Process</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure SLAs
- Configure Help Topics

<h2>Configure Roles</h2>
<p>
  <img src="https://github.com/user-attachments/assets/dbaac814-5c76-4aa6-8392-ae3de5eede2b" width="75%" alt="osTicket Config"/>
</p>
<p>
Initial login will use your admin account that you created in the Help Desk setup. We will create a role for Supreme Admin, that will have access to all permissions. This will be done in the "Roles" page of the "Agent" tab in the Admin Panel.
</p>
<br />

<h2>Configure Departments</h2>
<p>
  <img src="https://github.com/user-attachments/assets/38660853-7405-4a95-9a63-b57cf1561b4c" width="75%" alt="osTicket Config"/>
</p>
<p>
The Departments page is also accessed in the Agents tab. We will add a new Department named SysAdmins that will be a Top-Level Department.
</p>
<br />

<h2>Configure Teams</h2>
<p>
  <img src="https://github.com/user-attachments/assets/4cbe129a-c8e7-48e6-a78f-3c56d47dfeb3" width="75%" alt="osTicket Config"/>
</p>
<p>
The Teams page is also accessed in the Agents tab. We will add a new Team called "Online Banking
</p>
<br />

<h2>Configure Agents</h2>
<p>
  <img src="https://github.com/user-attachments/assets/791e9024-3b2b-450b-b252-ddcb7b201fcb" width="75%" alt="osTicket Config"/>
</p>
<p>
In order for different Admins and Support staff to be able to log in, we need new Agents to be added. We can do this by clicking the Agents tab right next to Teams, and selecting "Add New Agent." In here we can put in all the info and logins for the Agent, as well as configure their access, permissions, and team assignment.
</p>
<br />

<h2>Configure Users</h2>
<p>
  <img src="https://github.com/user-attachments/assets/85f5ec27-d9c0-4be3-8c0f-b9efbbab9fd3" width="75%" alt="osTicket Config"/>
</p>
<p>
We will add a couple example Users who will be able to log in to the osTicket system to submit tickets of their own. We can do this by clicking over to the Agent panel, going into the Users tab, and selecting "Add User." After entering the user's info, I am setting their password for them and not requiring a password change on login, but in normal situations it would be a good idea to allow Users to set their password.
</p>
<br />

<h2>Configure SLAs</h2>
<p>
  <img src="https://github.com/user-attachments/assets/b3f4b799-0d2f-4c80-8307-5282ac4f3c0f" width="75%" alt="osTicket Config"/>
</p>
<p>
Under the Manage tab, we can navigate to the SLA page, where we will create 3 new SLA's to prioritize tickets into different levels of urgency. For our intents and purposes these are named Sev-A, Sev-B, and Sev-C.
</p>
<br />

<h2>Configure Help Topics</h2>
<p>
  <img src="https://github.com/user-attachments/assets/60ffad9c-32fb-4cb3-99ae-92d801bf8cff" width="75%" alt="osTicket Config"/>
</p>
<p>
Help Topics are categories that Users can select when making tickets to help with organization on our end. We will make some new help topics by navigating to the "Help Topics" page under "Manage" adn entering each one individually.
</p>
<br />
