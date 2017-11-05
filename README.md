# Admin_SFTP-Monitor-V2.4
Monitor FTP site is working

--------------
Install Steps;
--------------
1. Create FTPMonitor Folder at any location
2. copy below files to newly created folder
	2.1 FTPMonitor.exe
	2.2 FTPMonitor.exe.config
	2.3 WinSCP.exe
	2.4 WinSCPnet.dll
3. Create folder: C:\Program Files (x86)\WinSCP
4. Copy WinSCPnet.dll, WinSCP.exe to C:\Program Files (x86)\WinSCP
5. Use text editor, open FTPMonitor.exe.config
6. Check or update file path *** DO NOT CHANGE ANY TAG NAME ***
7. Run FTPMonitor.exe
8. setup FTPMonitor.exe at task schedular(run every 10 minutes, 24x7)

--- Conditions ---
1. <configSections> should located before <appSettings> tag
2. you may change any value at anytime except '<system.net>' tag and it will be applied next connection
3. intervals is loaded only once in loading time and you may change it
4. you may change 'logging' tag from/to false/true
5. 'enablessl' tag is not supported by DOTNET 3.5 version,
   (from 4.0: enablessl can be used 'network' tag)
6. sessionlog will be created only if connection is made

---Version 2.2---
1. Creates text log file
