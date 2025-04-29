<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This demonstration outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: Initial osTicket Installation](https://youtu.be/p4DydgvwAOU)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

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
  <img src="https://github.com/user-attachments/assets/dbaac814-5c76-4aa6-8392-ae3de5eede2b" width="60%" alt="osTicket Config"/>
</p>
<p>
Initial login will use your admin account that you created in the Help Desk setup. We will create a role for Supreme Admin, that will have access to all permissions. This will be done in the "Roles" page of the "Agent" tab in the Admin Panel.
</p>
<br />

<h2>Configure Departments</h2>
<p>
  <img src="" width="60%" alt="osTicket Config"/>
</p>
<p>
The Departments page is also accessed in the Agents tab. We will add a new Department named SysAdmins that will be a Top-Level Department.
</p>
<br />

<h2>Configure Teams</h2>
<p>
  <img src="https://github.com/user-attachments/assets/4ea07d50-57fb-4332-8ee8-4d05a95d5abb" width="60%" alt="osTicket Config"/>
</p>
<p>
Next, we need to install Visual C++ Redistributable and IIS URL Rewrite Module. These are 2 things we need on the device to make everything work together.
</p>
<br />

<h2>Configure Agents</h2>
<p>
  <img src="" width="60%" alt="osTicket Config"/>
</p>
<p>
We will need to install PHP for Windows in order to be able to configure PHP Extensions for osTicket later. To do this, create a new directory in Windows(C:) named "PHP" and extract the zipped folder with the PHP installation files to it. This can be found at https://www.php.net/downloads. After that, we register the PHP version within the PHP Manager in IIS Manager by navigating to php-cgi.exe.
</p>
<br />

<h2>Configure Users</h2>
<p>
  <img src="" width="60%" alt="osTicket Config"/>
</p>
<p>
Before installing osTicket, it is best to already have an SQL server and UI installed. We'll be using MySQL as the server and HeidiSQL as the UI. When installing MySQL, I am using username and password "root". Inside of HeidiSQL, create a new database and name it osTicket.
</p>
<br />

<h2>Configure SLAs</h2>
<p>
  <img src="" width="60%" alt="osTicket Config"/>
</p>
<p>
Now we are installing osTicket. To do this, open C: > inetput > wwwroot, then in your osTicket installation file zip folder, drag the "upload" folder into wwwroot. Rename "upload" to "osTicket". From this osTicket folder navigate to the "include" folder and rename "ost-sampleconfig.php" to "ost-config.php." At this point we can go into IIS Manager, stop and start the server to refresh it, then navigate to Sites > Default Web Site > osTicket, click Browse on the right hand side and it will open up osTicket in the browser.
</p>
<br />

<h2>Configure Help Topics</h2>
<p>
  <img src="" width="60%" alt="osTicket Config"/>
</p>
<p>
To set up some recommended extensions for osTicket, open up PHP Manager within IIS Manager, select Enable or disable an extension under PHP Extensions, and enable, php_imap.dll, php_intl.dll, and php_opcache.dll, then refresh the browser and click continue on osTicket.
</p>
<br />
