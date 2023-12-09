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

- Configure roles
- Configure departments
- Configure teams
- Allow anyone to create tickets 
- Configure agents (associates)
- Configure users (customers)
- Configure SLAs
- Configure help topics 

<h2>Configuration Steps</h2>

Roles are the permissions granted to agents per department that they have access to. Each Role has a set of permissions that can be checked or unchecked for agents given that role in association with a department they have access to. An unlimited number of roles can be created and assigned to Agents with access to various departments. 

<p>

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/a3e52986-1ef5-4b5f-8fdb-ef75c5603133)


</p>
<p>
To modify or add new roles in osTicket, follow this path: admin panel > agents tab > roles 
</p>
<br />

I added a supreme admin role that gave me full access and permissions within the system. Within the window of "Permissions" tab I checked all the boxes in the "Tickets", "Tasks", "Knowledgebase" tabs. 

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/e08af0ca-1ecb-46ff-9b52-43220daae320)

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/44c0f46f-909b-4f84-a147-0efbaae703e6)

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/5c640d47-8008-4fee-9c19-10e9740736b3)

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/2fe440e3-eefe-4f9a-b45d-cfee3a4aa95e)







Departments in osTicket are used to classify agents' visibility of the tickets in the help desk system. They are used to organize agents into a group that works with specific sections of the organization and given different access and permissions from each other to make sure their work does not overlap.   

<p>

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/9e8d9158-fb9f-4db8-ac2c-4e33e71de2aa)


Once I was in the "add a new department" screen I created the "System Administrators" department.

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/2c006bbb-026c-4f3e-ae87-08e599317008)







<p>

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/b1178594-1d80-49bd-aecb-e1b3f6c6e0c5)


</p>
<p>
The team feature provides the ability to group staff members together (e.g across different departments) for the purpose of ticket assignment (manual or auto). Teams allow an organization to assign agents to different teams to help resolve issues within their scope of expertise. 
(e.g. A team of agents pulled from different departments that are experts in networking)
</p>
<br />

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/549d2a89-d0a4-4bc9-9d5b-49f194880220)


In osTicket, agents are given access to the help desk with the intent to respond and resolve the tickets for end users. I was able to configure the osTicket settings so that anyone had permission to create a ticket. 

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/1847a5a1-539c-4627-be1b-13526f8d5aa7)

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/ee640e07-f130-46e6-9436-0d329d915a34)

I had to make sure the "Registration Required" box was unmarked. 

<p>

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/d26aa4ab-25af-49c1-92fa-d2d6bd5f0b40)


</p>
<p>
I decided to create two agents, Jane and John. Once inside the window of "add a new agent", I added Jane first without the option to reqire password update and email password reset. I added her to the department of system administrators and gave her supreme admin permissions. I also gave her extended access to the support department so she is able to resolve and see tickets in the queue and added her to the Level II team.  

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/b611eed8-f0a6-421d-acf2-b9c2ce0ee0c9)

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/866f7198-6c66-4d23-bd6f-ddfcfa32d650)

![image](https://github.com/jonathansantacruz3/post-install-config/assets/151465848/8ca2ee08-b457-4f19-9e6e-d9fbe666143f)

I repeated the process with John's account, except, instead of giving him full access and permissions I added him to support and gave him enough permissions to do his support job. 

</p>
<br />

Users are the ticket owners of the tickets in the help desk. In other words they are the customers needing assistance in resolving a a tech related issue.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

SLA Plans or Service Level Agreement provide a length of time in which the help desk Administrator expects tickets to be closed.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

Help Topics will determine what Department the ticket is routed to which will determine which Agents have access to the ticket. The Help Topic also can determine other configurations of the ticket, such as the ticket’s SLA (or Service Level Agreement) and priority of a ticket, i.e. Emergency to Low.

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />


