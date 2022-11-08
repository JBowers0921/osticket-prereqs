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

- Active subscription in Azure
- Create a Resource Group 
- Create a Virtual Machine and connect to it remotely
- Enable ISS and Web Platform
- Configure Permissions
- Istall osTicketing System

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/PnNfAFL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In your browser, go to portal.azure.com and create a subscription. Next, create a Resourse Group (RG) by going to the search filed and typing in "resource group".
</p>
<br />

<p>
<img src="https://i.imgur.com/NG6aeRT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 In the middle of the screen, click on "create resource group". Next screen, name your Reseource Group (RG) and select a region. Select "review & create" and then "create" at the botton.
</p>
<br />

<p>
<img src="https://i.imgur.com/wfw51IG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After validation, your resource group will be displayed.
</p>
<br />
<img src="https://i.imgur.com/aORatls.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In order to create a virtual Machine(VM), from the Azure portal search field, type in virtual machine and press enter. On the next screen, select +Create as shown above.
</p>
<br />
<img src="https://i.imgur.com/W8I72gB.png " height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The next screen should be filled out similar to the example above. Be sure to select the Resource Group (RG) that you created in the previous step. Select the region and size accourding to your needs and location. Write down your username and password. You will need them for other processes.
</p>
<br />
<img src="https://i.imgur.com/YJDwLBI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This is the bottom of the previous page. Check the box under "Licensing" and then "Next:Disks, Next:Networking " Leave the defauld settings "as-is". Select "Review+Create". After your Validation has passed, select "Create".
</p>
<br />
</p>
<br />
<img src="https://i.imgur.com/TDx139B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Please wait while your VM is deploying.
</p>
<br />
</p>
<br />
<img src="https://i.imgur.com/2ByALX4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Return to your home screen, select the Virtual Machine icon to view the VM you created.
</p>
<br />
</p>
<br />
<img src="https://i.imgur.com/UBDynBY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
If you have not done so already, download/install the Remote Desktop Connection app onto your PC and pin it to your task bar. Return to Azure and open your VM1 and look to the right of the screen to locate your Public IP address. Copy it and open your Remote Desktop Connection App.
 
</p>
<br />
</p>
<br />
<img src="https://i.imgur.com/y6Ly5d5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 
Paste the copied Public IP address from VM1 into the Computer field and Click "connect" and follow the promps on the pop up windows to connect to VM1.
</p>
<br />
<p>
<img src="https://i.imgur.com/LnNfH4i.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 
You are now inside of VM1.
</p>
<br />

<p>
<img src="https://i.imgur.com/TVD2kOv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 
From inside of VM1, your next installation will be Internet Information Service (IIS). Open your control panel. Select Programs>Programs and Features> Turn Windows features on or off. On this pop up window, select IIS and then "OK"
</p>
<br />
<p>
 <img src="https://i.imgur.com/ehPOJhE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
 Open a Microsoft Edge browser and copy and paste the link for the installation files from your shared google drive.
</p>


<img src="https://i.imgur.com/HzCVuRP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<<p>
 
From your google drive documents, download and install Web Platform Installer inside of VM1.

 <br />

 
<img src="https://i.imgur.com/OEqgmSq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<<p>
 
From the Windows start menu, search for the Web Platform Installer and click on the app to open it.
</p>


<img src="https://i.imgur.com/iF4YIGS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 
 
In the search field, type MySQL 5.5 and then search. When it appears, select "Add".
</p>
<br />
<img src="https://i.imgur.com/bXYePTs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, in the same search field, type "PHP" and enter. Sort/Filter by name. Scroll down to where PHP begins and start adding all the simple version of x86 from 5.6.31 x86 to 7.3.25 x86. Select "Install"
</p>
<br />

<img src="https://i.imgur.com/mM1ooMd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 
The next pop-up window will require you to enter your password two times and click "Continue". Wait for the installation to stop.
</p>
<br />

<img src="https://i.imgur.com/vHqS7X5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 
In the next pop-up window, select "I Accept" to continue".
</p>
<br />
<img src="https://i.imgur.com/h6ksiB0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
You will see which programs failed installation. DO NOT CLICK FINISH yet. Return to your google drive files and download and install PHP manager and Microsoft C++ in order to fix any files that failed to install. 
 
 Go back to the Web Platform Installer and select "Finish". 
 
 
 Now you are ready to install osTicket v 1.15.8.
  </p>
<br />
<img src="https://i.imgur.com/qFwkh2X.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 From your google drive files, download and install osTicket. Go to your system downloads and right-click on osTicket. Select Extract All>Extract and wait for the process to finish.
</p>
<br />
<img src="https://i.imgur.com/AH2eJYr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go back to the download folder and open the extracted folder and find the folder named "upload". Copy and paste the "upload" folder into "This PC > Windows (C:)inetpub > wwwroot"  (c:\inetpub\wwwroot).
 Next, while still within the "wwwroot" folder, rename the "upload" file to "osTicket".
</p>
<br />
<img src="https://i.imgur.com/lc28wA6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/6axEaEY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the windows start menu and open the IIS app. Select the Restart icon in order to refresh the app. 

On the same screen, in the upper left area under Connections, go to Sites>Default Web>osTicket. Click on the osTicket folder in order to see "Browse*.80" on the right under "Browse Folder". Click on it and it will open the osTicket Installer window in Microsoft edge see Below:
 
 <img src="https://i.imgur.com/bi6gCPe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
</p>
<p>
 <img src="https://i.imgur.com/FkcpNdP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 </p>
<p>
To insure all extensions are Enabled in IIS: Go back to IIS > sites > default > osTicket and double click on the PHP Manager Icon.

</p>
<br />
<img src="https://i.imgur.com/ANzSKd8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open the PHP icon and select "Enable or Disable an extension. Enable the following: php_imap.dll, php_intl.dll and php_opcache.dll
</p>
<br />
<p>
 <img src="https://i.imgur.com/NjuRg8Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 </p>
<p>
Go back to your osTicket Installer window and observe the changes.
Next, go into C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php and rename the ost-sampleconfig.php file to ost-config.php

</p>
<br />
 <img src="https://i.imgur.com/KP2xKiH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 </p>
<p>
Finally, you need to assign permissions in ost-config.php. While you still have the "include" file open, scroll down to ost-config.php and right-click. Go to Properties > Security > Advanced >and click "Disable Inheritance" and then "Remove all inherited permissions from this object".
</p>
</p>
<br />
 <img src="https://i.imgur.com/sO2VUBh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 </p>
<p>
On the next pop-up screen: Select "Add", then "Select a principal", then type in the field "everyone", then click on "check names" then click "ok". This pop-up window will close.
</p>
</p>
<br />
 <img src="https://i.imgur.com/Y9NjpWS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 </p>
<p>
On the next pop-up screen: Put a check mark in the "Full Control" box, then "Ok". This pop-up window will close. Click "Ok" on the remaining open ost-config.php pop-up windows to close them out.
<br />
</p>
</p>
<br />
 <img src="https://i.imgur.com/gxPUBZl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 </p>
<p>
Next, return to your osTicket Installer browser to finish setting it up. Click "Continue" at the bottom. The screen above will display. On this screen, fill in the fields shown in the example above. STOP after retyping your password. 

</p>
</p>
<br />
Now, download and open "HeidiSQL" from your google shared lab files. Open the file and follow the promps install/launch it. 
</p>
</p>
<br />
 <img src="https://i.imgur.com/LVqFXrr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 </p>
<p>
When the new window pops up (HS Session Manager), click "+New " and enter your password for root from the instructions and select "Open"
<br />
</p>
</p>
 <img src="https://i.imgur.com/T0caIc0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/CeyuqGu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 </p>
<p>
On the Next window that pops up (HS Unnamed), right-click "Unnamed" > "Create new" > Database. Enter a name for the database called "osTicket"  and select "OK".  You will see it created in the list under Unnamed on the left. Close the window.
<br />
<br />
 <img src="https://i.imgur.com/EFj70AI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 </p>
<p>
Return to the osTicket Installer in your browser to complete the Database Settings section at the bottom. Fill in the "MySQL Database", "Username" and "Password" fields as shown above and selct "Install Now". You will see "Doing Stuff" message.
<br />
</p>
</p>
<img src="https://i.imgur.com/rleFyCg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 </p>
<p>
If there are no errors, you will see the Congratulations message on the osTicket Installer browser.  Finish up by removing the setup folder and it's contents from C:\inetpub\wwwroot\osTicket\setup. Then finally, set permissions to “Read” only in : C:\inetpub\wwwroot\osTicket\include\ost-config.php.
