![image](https://github.com/user-attachments/assets/aac2a0a3-bbae-4ee1-b484-b51eb971579e)<h1>osTicket - Prerequisites and Installation</h1>

- <b>This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket</b>

<h2>Environments and Technologies Used</h2>

- <b>Microsoft Azure</b> 
- <b>Virtual Machines</b>
- <b>Remote Desktop</b>
- <b>Internet Information Services (IIS)</b>
- <b>Description</b>

<h2>Operating Systems</h2>

- <b>Windows 10</b>

<h2>List of Prerequisites</h2>

- <b>Enable Internet Information Services (IIS)</b>
- <b>Install Web Platform Installer</b>
- <b>Install MySQL and setup username and password/b>
- <b>Install Microsoft Visual C++ 2009 Redistributable Package/b>
- <b>Configure permissions and install osTicket</b>

<h2>Installation Steps</h2>

![image](https://github.com/user-attachments/assets/ec44ed97-8329-42a7-8d10-5ed0fc8f1b6c)
- <b>Login to Microsoft Azure and create a Windows 10 virtual machine</b>

![image](https://github.com/user-attachments/assets/28272fde-e942-4c91-be03-a315bb34a3f4)
- <b>Open Remote Desktop Connection using your Windows virtual machine IP Address to connect</b>

![image](https://github.com/user-attachments/assets/669462f8-ec85-437a-a878-bd32a14d4cb5)
- <b>Open the control panel and go to programs>Turn Windows features on or off</b>
- <b>Select Internet Information Services>World Web Services>Application Development Features>CGI</b>

![image](https://github.com/user-attachments/assets/d3c9338b-4e91-47f6-a10b-7ceb5d9e6a33)
- <b>Select Common HTTP Features and turn on all features</b>

![image](https://github.com/user-attachments/assets/51608221-4cde-4df3-994d-887d54886747)
- <b>Open Edge from windows-vm and copy this link: https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6</b>
- <b>Download all the files</b>
- <b>Download PHPManager and rewrite_amd files</b>

![image](https://github.com/user-attachments/assets/e5de5074-6dd6-43c2-8766-90b2f068a500)
- <b>Create a new folder named PHP in the Windows C Drive</b>

![image](https://github.com/user-attachments/assets/3287dfe1-3f0e-42b9-8d25-6b2f3cfcf3e9)
- <b>Drag the PHP file from the installation files to the PHP folder</b>

![image](https://github.com/user-attachments/assets/fcc1e6da-a33f-4bae-8463-97e9c87a1341)
- <b>Run VC_redistribution from the installation files</b>

![image](https://github.com/user-attachments/assets/7fce934c-563d-4075-b3f3-2276023becc0)
- <b>Install MySQL Server</b>
- <b>Choose Typical and install</b>

![image](https://github.com/user-attachments/assets/0cfc3f36-0a51-4411-9ba8-bf25309ac608)
- <b>Choose Standard Configuration</b>

![image](https://github.com/user-attachments/assets/9ddf1814-5c0f-4fa7-9466-d23f2173fb55)
- <b>Execute</b>

![image](https://github.com/user-attachments/assets/f1f36298-cfd2-4655-89de-c2726e71f29b)
- <b>From your Windows virtual machine, search for Internet Information Services (IIS)</b>
- <b>Run as administrator</b>

![image](https://github.com/user-attachments/assets/9c7b0e1d-5b26-44a2-a12f-8ec6dd4a0e05)
- <<b>Select v-ost>PHP Manager>Register new PHP version and select php-cgi</b>

![image](https://github.com/user-attachments/assets/f7b1f420-4d9f-4e11-a670-6e7a71eeacfc)
- <b>Go to the installation files and select osTicket</b>
- <b>Drag the upload file to this file path</b>

![image](https://github.com/user-attachments/assets/6ef40445-90bb-41a5-bcd9-f6e75927c22c)
- <b>Rename the upload folder to osTicket</b>

![image](https://github.com/user-attachments/assets/53a4e1d4-1ebf-413d-b222-f9cb4ce7d958)
- <b>Go back to IIS and run as administrator</b>
- <b>Select v-ost>Sites>Default Web Site>osTicket</b>
- <b>Under Manage Folder, click Browse*80(HTTP)</b>


