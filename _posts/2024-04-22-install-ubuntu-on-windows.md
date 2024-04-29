---
title: Ubuntu installation with WSL
layout: default
date: 2024-04-22 7:00:00 +800
categories: BioInformatics
math: true
mermaid: true
---

# Basic ubuntu installation procedures
## System requirements
- OS: Windows 10 and above
- At least 25 GB free hard drive space
### Install Windows Subsystem for Linux (info retrieved from https://itsfoss.com)
- Search “windows subsystem for linux” from the Microsoft Store, then install (alternative: wsl --install in command prompt)
- Reboot to apply changes
### Install Ubuntu (retrieved from https://itsfoss.com)
- Search “Ubuntu” from the Microsoft Store, then install
- Reboot to apply changes
### In case these steps don’t work:
1.	Open Windows powershell (open as administrator)
2.	Enter this:
```console
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

3.	Restart
4.	Powershell (open as administrator): 
```console
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart 
```


5.	Restart
6.	Powershell: 
```console 
wsl --set-default-version 2
```

7.	Restart
### Configure the newly installed Ubuntu
- Provide a unix username and password
- Log-in, then update the installed Ubuntu by entering the following commands one by one:
		sudo apt update
			sudo apt full-upgrade
- Once update is finished, you are good to go.

























