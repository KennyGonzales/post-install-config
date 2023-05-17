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
  
Agents are granted access to the help desk to handle ticket responses and resolutions. When adding an agent to the help desk, they must be assigned a primary department and given a primary role for handling tickets and tasks routed to that department. Additionally, agents can be granted extended access to additional departments within the help desk and assigned different roles for those departments. These configurations can be managed in the Access tab of the agent's profile.

In the `Admin` panel, we'll go to `Agents` then `Add New`. From there, we are going to create and name two agents as **Jane** and **John**.  
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
</p>
<br />
<hr>
<p>
  
-Configure: [**Users**]
  
Users have the ability to create an account and log in to the help desk system. Once logged in, they can create new tickets or check the status of their existing tickets.  
  
In the `Admin` panel, we will click on `Users` then `Add New`. We will create two users and name them **Karen** and **Ken**.   
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
</p>
<br />
<hr>
<p>
  
-Configure: [**SLA**]
  
In osTicket, there are no limitations on the number of SLA Plans or Service Level Agreements that can be created. The purpose of an SLA Plan is to define the expected timeframe within which help desk administrators anticipate ticket closure.
  
In the `Admin` panel, we will click on `Manage` then `SLA`. We'll create three SLA plans and name them **Sev-A**, **Sev-B**, and **Sev-C**. The grace period and schedule for **Sev-A** will be **1 hour, 24/7**. For **Sev-B**, it's **4 hours, 24/7**. With **Sev-C**, it's **8 hours, business hours**. 
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
</p>
<br />
<hr>
<p>
  
-Configure: [**Help Topics**]
  
Help Topics play a crucial role in enhancing the end-user's help desk experience by facilitating efficient ticket assignment and prompt responses. You can create multiple Help Topics as required, and even organize them hierarchically for further categorization. For instance, you can nest Help Topics within each other, such as Human Resources and Human Resources/Payroll, to provide a more detailed breakdown of topics.
  
From the `Admin` panel, we'll click on `Manage` then `Help Topics`. We will create four help topics which will be **Business Critical Outage**, **Personal Computer Issues**, **Equipment Request**, and **Password Reset**.   
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
</p>
<br />

<p>
  
The selected items are all the tickets that we have created. The other are created by default.   
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<p align="right"> Next up, <a href="https://github.com/KennyGonzales/ticket-lifestyle"
>Ticket Lifestyle </a></p>
