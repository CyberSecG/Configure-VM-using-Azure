# Configure-VM-using-Azure
This is a step by step guide on how to create a virtual machine usine Azure.
# Creating a Virtual Machine
1)Go to https://azure.microsoft.com

2)Sign Up for a free 30 day subscription and create an account.

3)Once you have created your account and signed up for your free 30 Day subscripion you will go to your portal which you can access at anytime by going to portal.azure.com and logging in with your credentials.

4)Once in portal click on "resource groups" and then click "create".

5)Type in the the name of your resource group and select your desired region. Then click "Review+create" and once validation has passed click "create" once again. <img width="626" alt="Capture" src="https://user-images.githubusercontent.com/51884636/225787831-8fac1b77-d65d-4c76-87a2-ee29fe7c8542.PNG">

6)We will now head back to our home portal at portal.azure.com and we will click on the "Virtual Machine" Icon. Once in virtual machine we will click "create" and again click "Azure Virtual Machine."

7)Now you will name your Virtual Machine, select your region which should be the same region you chose for your resource group. For "Image" you will select your desired operating system (In this example I will choose the Windows 10 Pro, version 21H2 image. For "Size" you will select your desired cpu specs for your Virtual Machine.". For "Administrator account" you will create a username and password that is easy to remember as this is for a lab. You will have to check the box under licensing to advance. I would also like to mention for "Select inbound ports" have "RDP (3389)" selected as we will use this later to connect via RDP.<img width="619" alt="Capture1" src="https://user-images.githubusercontent.com/51884636/225793801-78ba921b-4dd1-4ffb-b99c-832bc4dce1be.PNG">

8)Click "Review+create", once validation has passed click "create" and wait for your Virtual Machine to be created.

9)Done, you now have a Virtual Machine.

# Remote Access using RDP
For Windows

1)Go to your portal home at portal.azure.com then click on "Virtual Machine" Icon.

2)Click on the virtual machine you just created and this will present you with and overview of information that has to do with your instance.

3)From here you will need the Public IP address of your virtual machine. Once you find it in the overview copy it down as you will need it to login via RDP.

4)Go to your window search bar in the start menu and search "Remote Desktop Connection" click it and open it.

5)Click on the "show options" button on the bottom left corner and then enter the public IP of your virtual machine into the computer field. You will also enter the username of the virtual machine you created. Then press "Connect."<img width="327" alt="Capture2" src="https://user-images.githubusercontent.com/51884636/225798815-327a8df0-95b2-455c-a3a2-cf0e1d09d3dc.PNG">

6)You will get a warning message saying this isn't safe, you can just bypass this message by clicking "Yes" as it will be safe. Once done, your vitual machine will open after some loading and waiting. Once prompted you can enter your username and password credentials and you will be welcomed by your virtual machine.

7)Done

For Mac

1)Download "RD Client" from the Apple store and yes it is free if your wondering.

2)Once installed open the app and click on the + sign and select "Add PC". Enter the public IP of your VM under user account. Type in your VM's username and password and then click "save". 

3)Once saved, click on the PC you just added and now your Virtual Machine will load on your Mac after some time waiting.

4)Done

FYI Remember to stop your VM and delete your VM and resource group within Azure so you don't run up a bill on a instance you forgot you had running. This can be a costly mistake if you are not careful.
