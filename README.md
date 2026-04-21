# osTicket-prereqs
<h1>osTicket - Prerequisites and Installation</h1>

<h2>Description</h2>
osTicket is implemented in this project to simulate a real-world IT support environment. This includes configuring a cloud-based virtual machine and setting up a help desk ticketing system. The project is designed to showcase practical skills relevant to entry-level IT support roles.
<br />


<h2>Environments and Technologies Used</h2>

- <b>Microsoft Azure - Virtual Machines</b>
- <b>Internet Information Services (IIS)</b>
- <b>Remote Desktop</b>
- <b>osTicket</b>

<h2>Operating Systems Used </h2>

- <b>Windows 10 / 11</b>

<h2>Program walk-through and demonstration:</h2>
The following steps outline the setup of a cloud-based IT environment using osTicket and the installation/configuration of osTicket.

### Create a Virtual Machine in Azure
<p align="center">
<img width="1410" height="382" alt="2026-04-20_16-10-13" src="https://github.com/user-attachments/assets/22345f96-8d6e-49b1-a5be-159d0916487b" />
</p>

### Connect to the Remote Desktop
<p align="center">
<img width="618" height="487" alt="log into remote desktop" src="https://github.com/user-attachments/assets/44c8a34a-4b8d-4d92-b564-483cf804626b" />
</p>

### Download osTicket and unzip file on desktop
<p align="center">
<img width="835" height="439" alt="Download osTicket" src="https://github.com/user-attachments/assets/77af7526-4a03-4c24-ab78-a85be238a838" />
</p>

### Enable IIS with CGI
<p align="center">
<img width="805" height="524" alt="Enable IIS with CGI" src="https://github.com/user-attachments/assets/adac6c04-83b8-49bf-901d-d2332e6270ce" />
</p>

### Install Required Files
Includes:
 - PHP Manager
 - Rewrite Module
<p align="center">
<img width="846" height="534" alt="Install PHP Manager" src="https://github.com/user-attachments/assets/81dd0a6d-9220-4295-8392-467721092e95" />
<img width="906" height="586" alt="Install Rewrite Module" src="https://github.com/user-attachments/assets/34880ce5-9316-41ef-9959-c98cb4cf8570" />
</p>

### Configure PHP Environment
 - Create `C:\PHP` directory
 - Extract PHP files
<p align="center">
<img width="744" height="466" alt="Create a new folder in Windows C" src="https://github.com/user-attachments/assets/7ec1fda0-61cb-4457-b823-d252a906b8e0" />
<img width="1098" height="491" alt="unzip php 738 file into new windows php folder" src="https://github.com/user-attachments/assets/9ca15a99-cee1-4d22-b7d1-5688049ae693" />
</p>

### Install more required files
Includes:
 - VC_redist
 - MySQL
<p align="center">
<img width="844" height="433" alt="Install VC redist from OsTicket Installation File" src="https://github.com/user-attachments/assets/25b95b0c-91b3-4f6f-8a43-460b1d3cd0ee" />
<img width="845" height="453" alt="Install mySQL from OsTicket Installation File" src="https://github.com/user-attachments/assets/4a73af2e-9cac-42b4-96e6-d1d850767fc8" />
</p>

### Register PHP within IIS
<p align="center">
<img width="675" height="443" alt="open iis as admin" src="https://github.com/user-attachments/assets/cc1f7719-a2ef-41c4-b77c-acd71dddfe1f" />
<img width="728" height="435" alt="register php 1" src="https://github.com/user-attachments/assets/c567b9c2-352c-4e94-8463-f6225a33abe6" />
<img width="1042" height="612" alt="register php 2" src="https://github.com/user-attachments/assets/4594d141-2949-418f-870c-6a539c54e5c9" />
</p>

### Deploy osTicket Files
- Extract osTicket into `C:\inetpub\wwwroot`  
- Rename `upload` folder to `osTicket`  

<p align="center">
<img width="979" height="439" src="https://github.com/user-attachments/assets/94e9c40c-b225-49c0-a5d3-dec2748d19d6"/>
<img width="658" height="300" src="https://github.com/user-attachments/assets/ea23fc7a-790d-4680-bb77-f1a7bc69edd4"/>
</p>

### Enable Required PHP Extensions
Enable:
- php_imap.dll  
- php_intl.dll  
- php_opcache.dll

<p align="center">
<img width="763" height="521" alt="enable or disavle extention" src="https://github.com/user-attachments/assets/b4c18134-3090-45f7-a17f-16fba51143bf" />
<img width="915" height="500" alt="emable extenstion" src="https://github.com/user-attachments/assets/787cf8d7-420b-462c-a159-a98d0ecd65b9" />
</p>

### Configure osTicket Settings
 - Rename `ost-sampleconfig.php` to `ost-config.php`
 - Set file permissions

<p align="center">
<img width="800" height="374" alt="rename file 1" src="https://github.com/user-attachments/assets/154d8c4a-2d14-47a6-8b7b-0d7ab439e3fe" />
<img width="778" height="351" alt="rename file 2" src="https://github.com/user-attachments/assets/de9a3353-fae5-4b17-a04a-bcc4e1919858" />
</p>

### Configure Databasa
Using HeidiSQL:
 - Create a new session
 - Create database `osTicket`

<p align="center">
<img width="948" height="589" alt="connect to session and create database" src="https://github.com/user-attachments/assets/46c3c541-38e7-4588-a4e2-d5f40212b48b" />
</p>

### Complete osTicket Installtion
Finalize setup in browser and log into the helpdesk system.

<p align="center">
<img width="683" height="628" alt="finish os browser setup 1" src="https://github.com/user-attachments/assets/4754a912-3b22-4701-a7f2-6552bc34c3e6" />
<img width="632" height="492" alt="final setup" src="https://github.com/user-attachments/assets/d1971753-3870-48f3-bcbf-42359f78b049" />
</p>
