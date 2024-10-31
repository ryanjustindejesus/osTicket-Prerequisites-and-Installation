<h1>osTicket - Prerequisites and Installation</h1>

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
- <b>Install MySQL and setup username and password </b>
- <b>Install Microsoft Visual C++ 2009 Redistributable Package </b>
- <b>Configure permissions and install osTicket</b>

<h2>Installation Steps</h2>

![image](https://github.com/user-attachments/assets/ec44ed97-8329-42a7-8d10-5ed0fc8f1b6c)
- <b>Login to Microsoft Azure and create a Windows 10 virtual machine</b>

![image](https://github.com/user-attachments/assets/28272fde-e942-4c91-be03-a315bb34a3f4)
- <b>Open Remote Desktop Connection using your Windows virtual machine IP Address to connect</b>

![image](https://github.com/user-attachments/assets/6796a496-b76d-41c4-9a61-e7c5d0c24da5)
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

![image](https://github.com/user-attachments/assets/8be3c3dc-6333-463e-aaf0-b819f7756156)
- <b>osTicket Installation</b>

![image](https://github.com/user-attachments/assets/15562ce3-6970-4d78-9947-96f6c6e8a634)
- <b>Go back to IIS and click PHP Manager</b>
- <b>Under PHP Extension, click enable or disable an extension</b>

![image](https://github.com/user-attachments/assets/e36e3006-6392-485c-9898-8698af52a11c)
- <b>Right click and enable php_imap</b>

![image](https://github.com/user-attachments/assets/74f2e888-15fd-4e8a-a7b1-aa90fd748f3d)
- <b>Enable php_intl</b>

![image](https://github.com/user-attachments/assets/4bb063fb-4fdb-4575-8adf-5d49bf0066ee)
- <b>Enable php_opcache</b>
- <b>Restart IIS</b>

![image](https://github.com/user-attachments/assets/361908c1-cc6c-47d3-91fd-bd846d7bb41a)
- <b>Navigate to osTicket and click include</b>

![image](https://github.com/user-attachments/assets/f5510708-6304-4b19-abda-9b6a8827065d)
- <b>Rename ost-sampleconfig.php to ost-config.php</b>

![image](https://github.com/user-attachments/assets/c6b22e58-a97f-4587-b99a-8e1ea432c949)
- <b>Right click ost-config.php and select properties</b>
- <b>Select Security>Advanced</b>

![image](https://github.com/user-attachments/assets/125183b6-f748-4a0a-aa01-d8c4194dcb0b)
- <b>Select Disable inheritance and Remove all inherited permissions from this object</b>
- <b>Click Add</b>

![image](https://github.com/user-attachments/assets/2a9710cc-a166-414a-8fcf-7ff0887166ef)
- <b>Select a principal and type Everyone</b>
- <b>Click Ok</b>

![image](https://github.com/user-attachments/assets/484ff7ea-f554-408c-ad9a-ba8be72e3dfc)
- <b>Select Full Control</b>

![image](https://github.com/user-attachments/assets/5fd66be4-0bb5-4be8-9224-19ff517ccf59)
- <b>osTicket updated/b>
- <b>Click continue</b>

![image](https://github.com/user-attachments/assets/6ea83228-cced-457d-9a1e-e93eca6be705)
- <b>Fill out the information and click Install Now</b>

![image](https://github.com/user-attachments/assets/fed676a3-abf3-4bf1-a19a-9e5a2984857f)
- <b>osTicket installed</b>

![image](https://github.com/user-attachments/assets/25063c13-07ba-4992-932e-f97a02842aad)
- <b>Go to the installation files and setup HeidiSQL</b>

![image](https://github.com/user-attachments/assets/594796bc-f34c-459a-86a4-8941ab5daf57)
- <b>HeidiSQL installation complete</b>

![image](https://github.com/user-attachments/assets/44f29231-959b-49fd-94a9-1e62a80ae761)
- <b>Click skip</b>

![image](https://github.com/user-attachments/assets/63e090c3-eac9-4866-8488-784c68a5bf0c)
- <b>Click New</b>
- <b>User: root</b>
- <b>Databases: osTicket</b>
- <b>Click save and Open</b>

![image](https://github.com/user-attachments/assets/b34c1653-a138-4da6-af59-376e36fe6357)
- <b>HeidiSQL Database</b>

![image](https://github.com/user-attachments/assets/b1cf340a-5c14-4694-b022-9cfcb18b6011)
- <b>Open Edge browser and go to this link: http://locahost/osticket/scp/login.php</b>

![image](https://github.com/user-attachments/assets/dcbbe744-057d-4e54-a2ce-7c3a1cc3e053)
- <b>Navigate back to the include file path</b>
- <b>Right click ost-config.php and select properties</b>
- <b>Click advanced and select everyone</b>

![image](https://github.com/user-attachments/assets/f6f0ba87-04f6-4227-a0d7-2ff35fd50c23)
- <b>Select Read only permissions</b>
- <b>Select Ok>Apply>Ok</b>

![image](https://github.com/user-attachments/assets/920f83a0-03bb-4286-a699-6c40bd25167b)
- <b>Dete the setup folder from the osTicket folder</b>

![image](https://github.com/user-attachments/assets/380aa69a-730a-42fe-a361-f9651fa5cb49)
![image](https://github.com/user-attachments/assets/f49cc9d9-35a0-4a72-80ae-8f0f0cc68a6f)
- <b>Login to osTicket</b>

