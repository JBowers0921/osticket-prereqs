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
<p>
From your google drive documents, download and install Web Platform Installer inside of VM1.
</p>
<br />
