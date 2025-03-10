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

- Set up virtual machine with azure, run Windows 10 with at least 4vCPU's
- Within the VM (osticket-vm), download the osTicket-Installation-Files.zip and unzip it onto your desktop
- Enable IIS in Windows WITH CGI
World Wide Web Services -> Application Development Features -> [X] CGI
- From the “osTicket-Installation-Files” folder, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi),
-From the “osTicket-Installation-Files” folder install the Rewrite Module (rewrite_amd64_en-US.msi)
Create the directory C:\PHP
From the “osTicket-Installation-Files” folder, unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder
From the “osTicket-Installation-Files” folder, install HeidiSQL.
Open Heidi SQL
Create a new session, root/root
Connect to the session
Create a database called “osTicket”


<h2>Installation Steps</h2>

<![Screenshot 2025-02-20 142009](https://github.com/user-attachments/assets/1e0be575-cfc7-4331-a880-67dd5b951fa0)

This first step is the step that begins the entire lab! I use Microsoft Azure to be able to do this lab without dirtying up my physical computer. As shown in the picture I am creating a virtual machine that I will later take the public IP address from, to then connect through remote desktop. As listed in the steps I begin with creating this virtul machine, in order to do this I selected "Windows 10" and accommodated it with 4 vCPU's.
</p>
<br />

<p>


![Screenshot 2025-02-20 181008](https://github.com/user-attachments/assets/1f2031c9-7006-4ef0-8970-cc88d6b2d542)
![Screenshot 2025-02-20 183300](https://github.com/user-attachments/assets/30f208dd-beb4-4733-91c0-e93a789e61fa)

This is now the unzipping proccess where I first download files within the virtual machine then open up my file explorer, I then go to my download tab and drag the file that I just downloaded onto the desktop. This is the "unzipping" process. Once downloaded I then right click the file thats presented on my desktop and select "extract all". After extracting the files I then go into them and enable IIS as well as PHP. Doing this will allow me to operate the OsTicketing system.
</p>
<br />

<p>

![Screenshot 2025-02-21 124318](https://github.com/user-attachments/assets/2fa48d3c-ee5b-4838-a9f1-fa995277c634)

![Screenshot 2025-02-21 125208](https://github.com/user-attachments/assets/a2675cca-1562-4f7f-aeb0-9a6495ec93da)

Now you've downloaded your OsTicketing System database.
</p>
<br />
