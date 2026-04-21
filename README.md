# osTicket-prereqs
<h1>osTicket - Prerequisites and Installation</h1>

<h2>Description</h2>
osTicket is implemented in this project to simulate a real-world IT support environment. This includes configuring a cloud-based virtual machine, setting up a help desk ticketing system, and demonstrating how IT teams manage incoming requests, assign tickets, and resolve technical issues efficiently. The project is designed to showcase practical skills relevant to entry-level IT support roles.
<br />


<h2>Environments and Technologies Used</h2>

- <b>Microsoft Azure - Virtual Machines</b>
- <b>Internet Information Services (IIS)</b>
- <b>Remote Desktop</b>
- <b>osTicket</b>

<h2>Operating Sysmtes Used </h2>

- <b>Windows 10 / 11</b>

<h2>Program walk-through and demonstration:</h2>

<p align="center">
Create the Virtual Machine in Azure: <br/>
<img width="1410" height="382" alt="2026-04-20_16-10-13" src="https://github.com/user-attachments/assets/22345f96-8d6e-49b1-a5be-159d0916487b" />

<br />
<br />
Log into the Remote Desktop:  <br/>
<img width="618" height="487" alt="log into remote desktop" src="https://github.com/user-attachments/assets/44c8a34a-4b8d-4d92-b564-483cf804626b" />

<br />
<br />
Download osTicket and unzip file on desktop: <br/>
<img width="835" height="439" alt="Download osTicket" src="https://github.com/user-attachments/assets/77af7526-4a03-4c24-ab78-a85be238a838" />

<br />
<br />
Enable IIS with CGI:  <br/>
<img width="805" height="524" alt="Enable IIS with CGI" src="https://github.com/user-attachments/assets/adac6c04-83b8-49bf-901d-d2332e6270ce" />

<br />
<br />
Install PHP Manager from the osTicket Installation File:  <br/>
<img width="846" height="534" alt="Install PHP Manager" src="https://github.com/user-attachments/assets/81dd0a6d-9220-4295-8392-467721092e95" />

<br />
<br />
Install Rewrite Module from the osTicket Installation File:  <br/>
<img width="906" height="586" alt="Install Rewrite Module" src="https://github.com/user-attachments/assets/34880ce5-9316-41ef-9959-c98cb4cf8570" />

<br />
<br />
Create a new folder in Windows (C:):  <br/>
<img width="744" height="466" alt="Create a new folder in Windows C" src="https://github.com/user-attachments/assets/7ec1fda0-61cb-4457-b823-d252a906b8e0" />

<br />
<br />
Unzip PHP 7.3.8 file into the Windows (C):\PHP folder:  <br/>
<img width="1098" height="491" alt="unzip php 738 file into new windows php folder" src="https://github.com/user-attachments/assets/9ca15a99-cee1-4d22-b7d1-5688049ae693" />

<br />
<br />
Install VC_redist from the osTicket Installation File:  <br/>
<img width="844" height="433" alt="Install VC redist from OsTicket Installation File" src="https://github.com/user-attachments/assets/25b95b0c-91b3-4f6f-8a43-460b1d3cd0ee" />

<br />
<br />
Install MySQL 5.5.62 from the osTicket Installation File:  <br/>
<img width="845" height="453" alt="Install mySQL from OsTicket Installation File" src="https://github.com/user-attachments/assets/4a73af2e-9cac-42b4-96e6-d1d850767fc8" />

<br />
<br />
Open IIS as an Admin:  <br/>
<img width="675" height="443" alt="open iis as admin" src="https://github.com/user-attachments/assets/cc1f7719-a2ef-41c4-b77c-acd71dddfe1f" />

<br />
<br />
Register PHP from within IIS:  <br/>
<img width="728" height="435" alt="register php 1" src="https://github.com/user-attachments/assets/c567b9c2-352c-4e94-8463-f6225a33abe6" />
<img width="1042" height="612" alt="register php 2" src="https://github.com/user-attachments/assets/4594d141-2949-418f-870c-6a539c54e5c9" />

<br />
<br />
Unzip osTicket v1.15.8 unto the Windows (C):\inetpub\wwwroot:  <br/>
<img width="979" height="439" alt="unzip ostick file to root" src="https://github.com/user-attachments/assets/94e9c40c-b225-49c0-a5d3-dec2748d19d6" />

<br />
<br />
Rename "upload" folder to "osTicket":  <br/>
<img width="658" height="300" alt="rename upload to osTicket 1" src="https://github.com/user-attachments/assets/ea23fc7a-790d-4680-bb77-f1a7bc69edd4" />

<br />
<br />
In IIS, go to Sites --> Default Web Site --> osTicket --> open Browse*:80 on the right side <br/>
Make note of the extensions that are not enabled: <br/>
<img width="986" height="520" alt="in IIS go to site - default - osticket" src="https://github.com/user-attachments/assets/6a3a865b-ba64-4179-acae-6a2f499b8559" />
<img width="641" height="564" alt="note of ext not enabled" src="https://github.com/user-attachments/assets/afe763b0-a328-4afd-92ec-7f0708dbf7e7" />

<br />
<br />
Back in IIS, go to Sites --> Default Web Site --> osTicket --> open PHP Manager --> "Enable or Disable an extension"  <br/>
Enable the following; php_imap.dll, php_intl.dll, php_opcache.dll <br/>
Refresh browser to ensure extensions are enabled and working: <br/>
<img width="763" height="521" alt="enable or disavle extention" src="https://github.com/user-attachments/assets/b4c18134-3090-45f7-a17f-16fba51143bf" />
<img width="915" height="500" alt="emable extenstion" src="https://github.com/user-attachments/assets/787cf8d7-420b-462c-a159-a98d0ecd65b9" />
<img width="633" height="552" alt="refresh browser to ensure ext r working" src="https://github.com/user-attachments/assets/ab014f07-a652-405c-a8e0-52c3fe36e43e" />

<br />
<br />
In the Windows(C): \inetpub\wwwroot\osTicket\include folder, rename the file "ost-sampeconfig/php to "ost-config.php":   <br/>
<img width="800" height="374" alt="rename file 1" src="https://github.com/user-attachments/assets/154d8c4a-2d14-47a6-8b7b-0d7ab439e3fe" />
<img width="778" height="351" alt="rename file 2" src="https://github.com/user-attachments/assets/de9a3353-fae5-4b17-a04a-bcc4e1919858" />

<br />
<br />
Right click the file --> Properties --> Security --> Advanced Security --> Disable inheritance:  <br/>
<img width="1197" height="662" alt="assign permissions" src="https://github.com/user-attachments/assets/205730e2-a733-49d3-a253-2b497ebcb64e" />

<br />
<br />
In the same window -- click Add, this is where you can what groups have access  <br/>
<img width="889" height="625" alt="add permissions" src="https://github.com/user-attachments/assets/0f52bccc-1017-440d-9842-24eeb6f7add6" />

<br />
<br />
Back in the browser, click continute to move forward on osTicket setup:  <br/>
<img width="633" height="552" alt="refresh browser to ensure ext r working" src="https://github.com/user-attachments/assets/ab014f07-a652-405c-a8e0-52c3fe36e43e" />
<img width="624" height="624" alt="continue browser setup" src="https://github.com/user-attachments/assets/e646824c-ec94-48b7-8ff0-2cecb8dbe77f" />

<br />
<br />
Install HeidiSQL from the osTicket Installation File:  <br/>
<img width="964" height="572" alt="install heidi" src="https://github.com/user-attachments/assets/b22a39af-69f0-40e6-a027-3f25167fd218" />

<br />
<br />
Open Heidi SQL --> Create a new session and connect to it --> Create a database called "osTicket":  <br/>
<img width="948" height="589" alt="connect to session and create database" src="https://github.com/user-attachments/assets/46c3c541-38e7-4588-a4e2-d5f40212b48b" />

<br />
<br />
Finish setting up osTicket in the brower:  <br/>
<img width="683" height="628" alt="finish os browser setup 1" src="https://github.com/user-attachments/assets/4754a912-3b22-4701-a7f2-6552bc34c3e6" />
<img width="632" height="492" alt="final setup" src="https://github.com/user-attachments/assets/d1971753-3870-48f3-bcbf-42359f78b049" />

<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
