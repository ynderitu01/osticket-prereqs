<p align="center">

<p align="center">
  <img src="https://img.shields.io/badge/Cloud-Microsoft%20Azure-blue?logo=microsoftazure&logoColor=white" />
  <img src="https://img.shields.io/badge/OS-Windows%2010-0078D6?logo=windows&logoColor=white" />
  <img src="https://img.shields.io/badge/Web%20Server-IIS-lightgrey?logo=microsoft&logoColor=blue" />
  <img src="https://img.shields.io/badge/Database-MySQL-blue?logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/App-osTicket%20v1.15.8-orange?logo=helpdesk&logoColor=white" />
</p>


<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial demonstrates how to install and configure **osTicket v1.15.8** on a Windows 10 VM hosted in Microsoft Azure.  
It covers setting up IIS, PHP, MySQL, HeidiSQL, and completing the osTicket installation.   <br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>✅List of Prerequisites</h2>

- Azure Virtual Machine running Windows 10  
- Internet Information Services (IIS) installed  
- PHP Manager for IIS  
- Rewrite Module for IIS  
- MySQL Database
- Register PHP from within IIS
- Install osTicket-v1.15.8
- Install HeidiSQL
- Complete osTicket set up

<h2>Installation Steps</h2>

##Step 1: Create an Azure Virtual Machine with Windows 10 and connect using Remote Desktop. Make sure your Network Security Groups allow RDP. Then log into the VM with Remote Desktop.
</p>
<img width="700" alt="Azure VM" src="https://github.com/user-attachments/assets/01d2dee9-e759-4b39-9d0f-5879c7e7f14b" />  
<br />

##Step 2: Enable IIS by going to Control Panel → Programs → Turn Windows Features On or Off → and check Internet Information Services, World Wide Web Services, Application Development features, then CGI.
</p>
<img width="350" alt="IIS Setup" src="https://github.com/user-attachments/assets/3ccbad3f-0437-4dc1-b6b4-5a51d309cb01" />  
<br />

##Step 3: Install PHP Manager for IIS  
</p>
<p><img width="400" alt="PHP Manager" src="https://github.com/user-attachments/assets/7142cc37-8375-43b9-ae08-cbfe247706b7" />  
<br />

##Step 4: Install IIS Rewrite Module  
</p>
<img width="400" alt="Rewrite Module" src="https://github.com/user-attachments/assets/890ba926-4c12-42c6-9eaa-5206bda0cd95" />  
<br />
  
<p>
##Step 5: Download and install MySQL Server.  
</p>
<img width="400" alt="MySQL Setup" src="https://github.com/user-attachments/assets/109d1b0b-f8c2-4bd1-8dd2-cf9a5a32d818" />  
<br />

<p>
##Step 6: Open IIS as an Admin and Register PHP from within IIS. Then reload (Open IIS, Stop and Start the Server)
</p>
<img width="600" alt="Register PHP" src="https://github.com/user-attachments/assets/d29445fa-a1bd-41b9-84dd-68384a2f8dad" /> 
<br />

<p>
##Step 7: Install osTicket-v1.15.8. Copy osTicket-v1.15.8 upload folder into c:\inetpub\wwwroot and rename the upload folder to osTicket. Then reload IIS. (Open IIS Stop and Start Server)
</p>
<img width="600" alt="osTicket Install" src="https://github.com/user-attachments/assets/5e29266a-9418-4898-9a41-b44272b35eb7" />  
<br />

##Step 8: Install HeidiSQL Open HeidiSQL → Create session → Connect → Create database named `osTicket`.  
</p>
<p><img width="600" alt="HeidiSQL" src="https://github.com/user-attachments/assets/fac796b1-6384-4be6-a749-6fd26f4c8160" />  
<br />

<p>
##Step 9: Complete osTicket Setup In browser → Assign permissions → Click Install Now.  
</p>
<p><img width="600" alt="osTicket Setup" src="https://github.com/user-attachments/assets/9d061bd1-103c-495c-8d75-201a9bec322e" /> 
<br />

#🎉Done!  
You now have osTicket successfully installed on your VM.  
Next steps: configure departments, users, SLAs, and email piping for full help desk functionality.  




