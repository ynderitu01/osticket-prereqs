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

<h1># osTicket - Prerequisites and Installation 👩🏽‍💻</h1>
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

- Azure Virtual Machine running Windows 10, 4 vCPUs
- Remote Desktop Log in
- osTicket-Installation-Files
- Internet Information Services (IIS) installed  
- PHP Manager for IIS  
- Rewrite Module for IIS  
- MySQL Database
- Register PHP from within IIS
- Install osTicket-v1.15.8
- Install HeidiSQL
- Complete osTicket set up

<h2>Installation Steps</h2>

##Step 1: Create an Azure Virtual Machine with Windows 10, 4 vCPUs. Name the Virtual Machine osticket-vm and create user name and pasword.
</p>
<img width="700" alt="Azure VM" src="https://github.com/user-attachments/assets/01d2dee9-e759-4b39-9d0f-5879c7e7f14b" />  
<br />

##Step 2: Log into the VM with Remote Desktop using the VM Public IP address. 
</p> 
<img width="600" alt="Screenshot 2025-10-07 181642" src="https://github.com/user-attachments/assets/2b2b5052-ddaa-4e35-a6f5-2974beb74981" />
<br />

##Step 3: Within the VM (osticket-vm), download osTicket-Installation-Files.zip and unzip it onto your desktop. name the foler osTicket-Installation-Files.
We will use the files in this folder to install osTicket and some of the dependencies.
</p>
<img width="600" alt="image" src="https://github.com/user-attachments/assets/eb6fae71-1eac-4690-b202-c003510a6939" />
<br />

##Step 4: Enable IIS in Windows WITH CGI. Control Panel → Programs → Turn Windows Features On or Off → and check Internet Information Services, World Wide Web Services, Application Development features, then CGI.
</p>
<img width="350" alt="IIS Setup" src="https://github.com/user-attachments/assets/3ccbad3f-0437-4dc1-b6b4-5a51d309cb01" />  
<br />

##Step 5:From osTicket-Installation-Files install PHP Manager for IIS  
</p>
<p><img width="400" alt="PHP Manager" src="https://github.com/user-attachments/assets/7142cc37-8375-43b9-ae08-cbfe247706b7" />  
<br />

##Step 6:From osTicket-Installation-Files install IIS Rewrite Module  
</p>
<img width="400" alt="Rewrite Module" src="https://github.com/user-attachments/assets/890ba926-4c12-42c6-9eaa-5206bda0cd95" />  
<br />

##Step 7: Create the directory C:\PHP and unzip (php-7.3.8-nts-Win32-VC15-x86) From osTicket-Installation-Files into the C:\PHP
</p>
<img width="500"  alt="image" src="https://github.com/user-attachments/assets/f93a3a0c-30ef-449e-88a8-905071b59353" />
<br />

##Step 8: From osTicket-Installation-Files install VC_redist.x86.exe
</p>
<img width="500" alt="image" src="https://github.com/user-attachments/assets/a09506f0-6837-41c8-be31-2c18e45ad20d" />
<br />
##Step 9: From osTicket-Installation-Files download and install MySQL 5.5.62 (mysql-5.5.62-win32). Agree > Typical Setup > Launch Configuation Wizard (after install)> Standard Configuration> set User Name and Password.
</p>
<img width="400" alt="MySQL Setup" src="https://github.com/user-attachments/assets/109d1b0b-f8c2-4bd1-8dd2-cf9a5a32d818" />  
<br />

##Step 10: Open IIS as an Admin Register PHP from within IIS. Windows > IIS run as admin> PHP> php-7.3.8-nts-Win32-VC15-x86 > php-cgi. Then reload (Stop and Start the Server)
</p>
<img width="600"  alt="image" src="https://github.com/user-attachments/assets/2086f773-27f0-4026-8730-0b4bb5db0d80" />

##Step 11: Install osTicket-v1.15.8. From osTicket-Installation-Files unzip osTicket-v1.15.8 > copy upload folder into c:\inetpub\wwwroot and rename the upload folder to osTicket. Then reload IIS. (Open IIS Stop and Start Server)
</p>
<img width="600"  alt="image" src="https://github.com/user-attachments/assets/120b7ba8-5bef-4228-9864-4ac86e4a08ae" />
<br />

##Step 12: Browse osTicket. IIS > Site > Default Web site > osTicket. On the right click "Browse 80"
</p>
<img width="600"  alt="image" src="https://github.com/user-attachments/assets/3b90cfe2-c879-49d3-a64b-e47aff7bd6a3" />
<br />

##Step 13: Note some extentions on osTicket are not enabled. Go to IIS > Sites > Default > osTicket. Double Click PHP Manager and enable php_imap.dll, php_intl.dll, php_opcache.dll. Refresh the osTicket site in your browser, observe the changes.
<img width="700" alt="image" src="https://github.com/user-attachments/assets/7c8cabc2-9b4d-48ab-b1d4-63ff45455fe0" />
<br />

##Step 1: Install HeidiSQL Open HeidiSQL → Create session → Connect → Create database named `osTicket`.  
</p>
<p><img width="600" alt="HeidiSQL" src="https://github.com/user-attachments/assets/fac796b1-6384-4be6-a749-6fd26f4c8160" />  
<br />

##Step 13: Complete osTicket Setup In browser → Assign permissions → Click Install Now.  
</p>
<p><img width="600" alt="osTicket Setup" src="https://github.com/user-attachments/assets/9d061bd1-103c-495c-8d75-201a9bec322e" /> 
<br />

##🎉Done!  
You now have osTicket successfully installed on your VM.  
Next steps: configure departments, users, SLAs, and email piping for full help desk functionality.  




