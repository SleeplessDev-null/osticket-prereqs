<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>


-  Azure Virtual Machine
-  HeidiSQL
-  PHP Manager
-  osTicket v1.15.8
-  VC Redist
-  MySQL
-  Internet Information Services (IIS)
-  Rewrite Module
-  Link to the Installation files https://drive.usercontent.google.com/download?id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD&export=download


<h2>Installation Steps</h2>

<p align="center">
  First login to Microsoft Azure navigate to the search bar and look for resource group  :
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/First%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Name the resource group and select the region . Make sure to remember the region:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/first%20.1.5%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Navigate to the search bar and search for virtual machines. create a azure virtual machine, select the resource group you just created, name the VM, select the region, then the image which should be windows 10:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/Second%20step%201.5.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
after that set the username and password and don't forget to tick the box at the bottom. For this virtual machine you can keep everything default and review + create :
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/second%20step2.0.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Once this is done go to virtual machines, click on your VM and on the right copy the public ip address:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/Third%20step%201.5.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Now hold the windows key and press S to open your windows search, type remote desktop, when the window pops up paste the ip address and press connect. Then login with the username and password you set for the VM:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/Login%20to%20the%20windows%20vm.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
when you get logged in make your way to microsoft edge and download the install files for osTicket. once downloaded go to your downloads and extract the files, it can be in the downloads folder. and open the folder:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/osticket%20pre%20install%20files.PNG?raw=true" height="90%" width="80%"  />
<br /> 
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/Pre%20install%20files%20for%20osticket%201.PNG?raw=true" height="90%" width="80%"  />
   
</p>
