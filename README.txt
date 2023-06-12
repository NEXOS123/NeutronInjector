#Neutron Injection Manager Manual
User manual for the free version of NIM | C#
Difficulty: Intermediate
Coding Language: C#
Author: Likon

About NIM(Neutron Injection Manager):
It is Free to use, as long as you provide it into Credits
LoadLibraryA Injection
CS:GO-Only Injector
Semi-Fulll VAC-Bypass
While using NIM in your own project, if you folow all steps corectly, it will update itslef, you don't need your own server for updates or any other stuff

Requirements:
Visual Studio 2022/2019
.NET Framework v4+
Microsoft VC++ Installed
Minimum 32bit System
Encryption app(ex. ConfuserEx)
MergeAPP(ex. ILMerge)
Vedoo.VedooControls NuGet package v3
Stable Internet Connection
All applications/packages have their own Licence type,  you can get them from free from a secure sorce.

Step 1:
Create a new Project in Visual Studio, with the template: "Windows Forms App (.NET Framework C#)". In the Project Name enter your Injector name, such as "NeutronReplica". In the Location, choose the location you want to use for this project, in this example we are using: "D:\VS Apps". The solution name shoud be thee same as your Project Name. In the comboBox called "Framework", make sure it is selected ".NET Framework 4.7.2". Click on "Create".

Step 2:
After you created the project, go to Project > Manage NuGet Packages > Browse > Search for "Vedoo.VedooControls" and choose the version 3.0.1, then hit "Install". You will have to accept it's MIT Licence by pressing on "I Accept".

Step 3:
Wait for the installation to complete and close the NuGet Tab, returning to Form1.cs. Make your own design using Vedoo.VedooControls. Make sure to include a VedooCustomButton and rename it to "btnBrowseDLL" and it's text to "Browse DLL". You can add a status label, we will add one for this Manual. It's name is "lblStatus", and it's text is set to "None".

Step 4:
Dobble click on your "Browse DLL" button and use this code located on pastebin: https://pastebin.com/yBpAupL3
Password: Neutron123
You will need to add this under in your Form class: https://pastebin.com/pazWm5CB
Password: Neutron123

Step 5:
After you have done everything go to Project > Add new Item and choose "Application Manifest File (Windows Only)" DO NOT RENAME IT!
Then replace this line of code:  <requestedExecutionLevel level="asInvoker" uiAccess="false" />
With this one:  <requestedExecutionLevel level="requireAdministrator" uiAccess="false" />

Step 6:
Add this code to your app, to make sure that your users always have the last version of NIM.
You will need to click on Form1, in the properties window click on "Events" and select FormClosing and hit Enter, there you will need to add this code: https://pastebin.com/JQaBEFNj
Password: Neutron123

Step 7:
Change the build type from Debug > Release and hit Start.

Step 8:
After you have done this, it will ask for restart, but you can ignore it or hit on Restart, go to your application Folder path, ouers is: D:\VS Apps\NeutronReplica\NeutronReplica\bin\Release
And Copy your executable with Vedoo.VedooControls.dll to desktop in a folder.

Step 9:
Open ILMerge and drag + drop Vedoo Controls and your Injector there, make sure to choose a Output Path, click on "Merge!"

Step 10:
Take the Merged app into ConfuserEx and drop it there, go to "Settings" Tab, the on <Global Settings>, hit the +, select true, and the hit edit, on preset choose Agressive, if you go above, your app won't work. Press "Done", go to "Protect!" Tab and hit Protect, make sure to copy the output folder from the "Project" Tab.

Step 11:
Publish your Injector/keep editing and experimenting with it, sure, you can keep it for yourself.

KEEP IN MIND:
Always after you created the project, you will need to Merge and encrypt it, else someone else may copy your project.

Why Vedoo.VedooControls?
Thats what we found out to work the best, but you may use anything.
Im too lasy to do it myself, can i get the full project?
Yes, you can get it here: https://github.com/NEXOS123/NeutronInjector

READ THIS
This Manual is made by Likon, and we reserve the right to stop updating/complete reoving the public NIM from out GitHub. DO NOT SELL!
This Manual was hand-written and may have some typing errors.
