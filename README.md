<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine running Windows 10  
- Internet Information Services (IIS) installed  
- PHP Manager for IIS  
- Rewrite Module for IIS  
- MySQL Database
- Register PHP from within IIS
- Install osTicket-v1.15.8

<h2>Installation Steps</h2>

Step 1: Create an Azure Virtual Machine with Windows 10 and connect using Remote Desktop. Make sure your Network Security Groups allow RDP. Then log into the VM with Remote Desktop.
</p>
<p>
<img width="1445" height="702" alt="image" src="https://github.com/user-attachments/assets/01d2dee9-e759-4b39-9d0f-5879c7e7f14b" />
</p>
<br />

Step 2: Enable IIS by going to Control Panel → Programs → Turn Windows Features On or Off → and check Internet Information Services, World Wide Web Services, Application Development Feautures, then CGI.
</p>
<p>
<img width="347" height="357" alt="image" src="https://github.com/user-attachments/assets/3ccbad3f-0437-4dc1-b6b4-5a51d309cb01" />
</p>
<br />

Step 3: Install PHP Manager for IIS
</p>
<p>
<img width="671" height="564" alt="image" src="https://github.com/user-attachments/assets/7142cc37-8375-43b9-ae08-cbfe247706b7" /> 
</p>
<br />

Step 4: IIS Rewrite Module.
</p>
<p>
<img width="684" height="496" alt="image" src="https://github.com/user-attachments/assets/890ba926-4c12-42c6-9eaa-5206bda0cd95" />
</p>
<br />
  
<p>
Step 5: Download and install MySQL Server.  
</p>
<p>
<img width="680" height="547" alt="image" src="https://github.com/user-attachments/assets/109d1b0b-f8c2-4bd1-8dd2-cf9a5a32d818" />
</p>
<br />

<p>
Step 6: Open IIS as an Admin and Register PHP from within IIS. Then reload (Open IIS, Stop and Start the Server)
</p>
<p>
<img width="1495" height="941" alt="image" src="https://github.com/user-attachments/assets/d29445fa-a1bd-41b9-84dd-68384a2f8dad" />
</p>
<br />

<p>
Step 7: Install osTicket-v1.15.8. Copy osTicket-v1.15.8 upload folder into c:\inetpub\wwwroot and rename the upload folder to osTicket. Then reload IIS. (Open IIS Stop and Start Server)
</p>
<p>
<img width="1403" height="798" alt="image" src="https://github.com/user-attachments/assets/5e29266a-9418-4898-9a41-b44272b35eb7" />
</p>
<br />S
<p>
Step 8: 
</p>
<p>
<img width="1495" height="941" alt="image" src="https://github.com/user-attachments/assets/d29445fa-a1bd-41b9-84dd-68384a2f8dad" />
</p>
<br />

<p>
Step 9:
</p>
<p>
<img width="1495" height="941" alt="image" src="https://github.com/user-attachments/assets/d29445fa-a1bd-41b9-84dd-68384a2f8dad" />
</p>
<br />




