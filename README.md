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

- Log into osTicket Admin panel
- Configure Roles, Departments, & Teams
- Allow anyone to create tickets
- Configure Agents, Users, & SLA
- Design Help Topics

<h2>Configuration Steps</h2>

After logging into your helpdesk login page (http://localhost/osTicket/scp/login.php), it will take you to the **_agent_** panel. This displays the tickets for the helpdesk/admin that are created by the end users. 

<img src="https://i.imgur.com/0GC1PFq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p>
  
-Configure: [**Roles**]
  
Roles define the permissions granted to agents based on the departments they can access. Each role consists of a specific set of permissions that can be enabled or disabled for agents assigned to that role within their associated department. There is no limit to the number of roles that can be created, allowing for flexible assignment of roles to agents with access to different departments.  

In the admin panel, we will go to `Agents`, click on `Roles`, and we are going to create a new role called `Supreme Admin`. 
  
<img src="https://i.imgur.com/UrRMt0r.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
</p>
<br />

<p>
  
We can now proceed to enable permissions for this role. As the "Supreme Admin," we have chosen to enable all available permissions.
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<hr>
<p>

-Configure: [**Departments**]
  
Given that tickets are directed to specific departments in the help desk, there are numerous settings that can be configured for each department.
  
In the `Admin` panel, we'll click on `Agents` then `Departments`. When we add the new department, we will name that department **System Administators**. Keep the remaining fields at their default settings and take a moment to review the available options and selections to choose from.  
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
</p>
<br />
<hr>
<p>
  
-Configure: [**Teams**]
  
Teams enable the grouping of agents from various departments, allowing them to collaborate and address specific issues or users based on help topics or ticket filters.
  
In the `Admin` panel, we'll go to `Agents` then `Teams`. From there, we'll create two teams and name them **Level I Support** and **Level II Support**.    
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
</p>
<br />

<p>
  
-Allow anyone to create tickets in user settings
  
Enforcing user registration for ticket creation on the Help Desk serves the purpose of preventing random ticket submissions and limiting Users' access to the help desk.
 
In the `Admin` panel, we'll go to `Settings` then `User Settings`. For `Registration Required`, we are going to leave it **unchekced** for tickets being created with no restrictions/limitations. 
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<hr>
<p>
  
-Configure: [**Agents**]
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
  
Write here  
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
