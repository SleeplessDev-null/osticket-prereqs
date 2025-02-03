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
when you get logged in make your way to microsoft edge and download the install files for osTicket. once downloaded go to your downloads and extract the files, it can be in the downloads folder. Then open the folder:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/osticket%20pre%20install%20files.PNG?raw=true" height="90%" width="80%"  />
<br /> 
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/Pre%20install%20files%20for%20osticket%201.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />  
Now press and hold the windows key and press S to open up windows search and type control panel. click uninstall a program  and on the top left click on "Turn Windows features on or off " tick the boxes from the screen shot: 
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/Fourth%20step%20enable%20cgi.PNG?raw=true" height="90%" width="80%"  /> 
<br />
<br />
After this go back to the install files and run the installer for php manager keep everything default and install:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/5th%20step.PNG?raw=true" height="90%" width="80%"  />  
<br />
<br />
Now install IIS URL Rewrite Module keep everything default and install:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/6th%20step.PNG?raw=true" height="90%" width="80%"  />  
<br />
<br />
After this make your way to the your windows directory and make a "PHP" folder, make sure its capped and in the main directory like in the screenshot :
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/7TH%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Now go back to the install files and extract php-7.3.8-nts-Win32-VC15-x86.zip into the PHP folder you just created :
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/8th%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/8th%20step%201.5.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Next Install the VC_redist.x86 like with the last ones leave everything default and install:
<br />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/9th%20step.PNG?raw=true" height="90%" width="80%"  /> 
<br />
<br />  
Now install Mysql-5.5.62-win32.msi with this one follow the steps in the screenshots, NOTE: when you get to Service name, and password to use root only if this is for learning purposes. If you are using this for work make sure the service name and password is something you can remember and is unique.
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/10th%20step.PNG?raw=true" height="90%" width="80%"  />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/10th%201.5%20step.PNG?raw=true" height="90%" width="80%"  />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/10th%20step%202.0.PNG?raw=true" height="90%" width="80%"  />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/10th%20step%202.5.PNG?raw=true" height="90%" width="80%"  />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/10th%20step%203.0.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Once its installed go to windows search and type IIS and run as admin:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/11th%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
within IIS look for the php manager:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/12th%20step.PNG?raw=true" height="50%" width="40%"  />  
  
  

  
</p>
