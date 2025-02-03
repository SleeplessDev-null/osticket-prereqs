<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This Guide outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />



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


<h2>This a guide on how to install osTicket. Files included above. I hope to provide you with a pretty easy to follow guide and after this you will have a understanding on how to install it.  </h2>


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
<br />
<br />
Click on php manager and register new php version:
<br />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/13th%20step%20.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Now when it ask you to provide the path, you will link it to the php-cgi.exe inside of the PHP folder you made earlier:
<br />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/14th%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Once this is done go back to the IIS interface and on the right there should be a button to stop, start and restart. click stop then start to refresh everything:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/15th%20step.PNG?raw=true" height="50%" width="40%"  />
<br />
<br />
Make your way back to the install files and extract the osTicket-v1.15.8.zip, then go to your windows directory and follow this path c:\inetpub\wwwroot. Move the upload folder into the wwwroot folder and rename it to osTicket, make sure its spelled just like I have it  : 
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/16th%20step.PNG?raw=true" height="90%" width="80%"  />
<br /> 
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/17th%20step%20.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Now make your way back to the IIS interface and look on the left, follow this path in the connections tab, click on osTicket then look for browse 80 on the right side and click on it:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/18th%20step%20.PNG?raw=true" height="90%" width="80%"  />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/18th%20step%20.1.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
The webpage for osTicket should look like this.: 
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/19th%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />  
Some of the extensions need to be enabled so back in IIS we need to go to PHP manager and click on enable extension at the bottom. Enable the following , php_imap.dll, php_intl.dll, and php_opcache.dll:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/20th%20step%201.PNG?raw=true" height="90%" width="80%"  />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/20th%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
The osTicket page should now have the needed extensions enabled:
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/21st%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Now that this is done navigate back to your windows directory and follow this path C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php, inside of the include folder rename ost-sampleconfig.php to ost-config.php:
<br />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/22%20nd%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Now right click on ost-config.php and select properties, go to the security tab and click on advance , disable inheritance, and "Remove all inherited permissions from this object":
<br />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/23rd%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/23rd%20.1%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
After that click add, then select a principal, and in "Enter object name to select" type everyone. press ok and make sure all of the boxes are checked. Note you wouldn't put everyone in a real world use, Just for this guide:
<br />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/23rd%20step%20.2.PNG?raw=true" height="90%" width="80%"  />
<br />
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/23rd%20step%20.3.PNG?raw=true" height="90%" width="80%"  />
<br />
<br /> 
Now go back to the osTicket webpage, set up the help desk passwords, usernames, and emails. You don't have to use a real email but remember the passwords and usernames. Don't click the install button yet:
<br />
<br />   
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/24th%20step%20.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Now head back to installation folder for osTicket and run the installer for Heidi SQL. Once its installed let it launch :
<br />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/25th%20step%20.PNG?raw=true" height="90%" width="80%"  />
<br />   
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/25th%20step%20.1.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />  
when it opens click new at the bottom and create a new session and name it osTicket. On the right for user and password would put root and press open: 
<br />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/26th%20step%20.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
Now back in the osTicket webpage you can now put in the rest of the information and click install. and now you osTicket is installed:
<br />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/27th%20step%20.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />
To clean up a some files go back to your www.root folder and look for the osTicket folder. Inside delete the setup folder and you are done.
<br />
<br />  
<img src="https://github.com/SleeplessDev-null/osticket-prereqs/blob/main/Png/28th%20step.PNG?raw=true" height="90%" width="80%"  />
<br />
<br />




<h2>This concludes the installation of osTicket. I hope the guide was simple and understandable but of course there is more to setting up osTicket so this guide will be split into 3 parts.  </h2>
  





  
  
  

  
</p>
