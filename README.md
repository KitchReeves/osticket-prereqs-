<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>List of Prerequisites</h2>

- Item 1 Azure account
- Item 2 osticket instilation files
- Item 3 remote desktop connection app


<h2>Installation Steps</h2>
Step 1 create a VM with these settings on Azure
</p>
<p>

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/9487f7ef-5dc9-44ab-b95e-5a4bf0e829d6)

Step 2 access the VM with Remote Desktop

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/173384df-2565-4384-9269-016a9aed8b24)

Step 3 Open Control panal, > Programs > Turn Windows features on or off>
 and turn on all these specific features.

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/3ef10b9f-15b3-4170-9c44-67830fbe4cd2)

Step 4 download and install softwares onto VM 
link with all installs 
https://drive.google.com/drive/u/1/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6
You do need to do these in a specific order

install
![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/565e064c-cc69-4d79-afe5-345e6d549e94)

install
![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/7e9adba5-823e-4480-afe0-64e5b1385782)

</p>

Create PHP folder at Windows (C:) and extract the php-7.3.8-nts-win32 in there

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/49ac8877-2439-475f-bdd1-85aebfe3cf67)

<p>

install with typcal, and standard configuration

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/87139e8f-5db7-4bfd-af6b-97865787f1bf)

Step 5 open IIS Manager, go to PHP Mnager and register new PHP

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/50781c0f-1456-45d3-88f7-d7bc27d840d8)
![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/f2c5acc5-6adf-4c54-854c-ca40cf10ffd6)

Step 6  move "upload" folder to C:\inetpub\wwwroot and rename to "osTicket"

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/d88bed55-e2ab-4d74-af8b-3fb1c04154a8)
![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/72ecd1fd-5501-4a3a-bbb8-52302f3c2b92)

Step 7 Eneble Extions for OsTicket

php_imap.dill,

php_intl.dill,

php_opcache.dill

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/6768ac55-c1a9-470d-b8c9-29138fb9e0c0)

step 8 rename ost-sampleconfig.php to ost-config.php

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/1efb9924-65a8-4f1a-a4db-45281efee18d)

step 9 dissable inheritance and allow everyone full control

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/71c9ea0e-c76d-4e63-bcd3-6716de91c9e3)

step 10 install HeidiSQL and create session

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/2ac004fa-79ff-4916-b8eb-cd3ec9e86073)

step 11 opening OsTicket

select osTicket > click Brows *:80 (http)

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/9e767f4b-4523-43d5-99e0-6a50f678a066)
![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/40fdbc3d-1185-43ea-b0ea-78070458d421)

step 12 input needed info

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/02f8dda6-f3b1-4573-acf7-d4a4b9ac03ba)

step 13 set ost-config.php "permissons to read only" C:\inetpub\wwwroot\osTicket\include

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/cc302078-16e2-4db9-8a81-5052bc5ad3c7)

step 14 final delete "setup" folder

![image](https://github.com/KitchReeves/osticket-prereqs-/assets/158783649/00c7d0a0-122a-4369-96e3-0d870b7efac4)

view https://github.com/KitchReeves/OS-Ticket-config for configure set up



















