## <div align="center">Installation of Windows Subsystem for Linux (WSL) on Windows 11</div>
# <div align="center"><img src= https://technoresult.com/wp-content/uploads/2021/08/Install-WSL-using-cmd-feature-image.jpg align="center" width="600" ></img></div>
* #### WSL, or Windows Subsystem for Linux, is a compatibility layer developed by Microsoft that allows users to run a Linux distribution natively on Windows. It provides a Linux environment within Windows without the need for a virtual machine or dual-boot setup.
* #### Install Your favourate linux distro on Windows 11 such as kali, Ubuntu, Arch.

## Step 1: Enable the Windows Subsystem for Linux (WSL) Feature.

#### Press ```Win``` + ```R``` key On Keyboard type ```optionalfeature```. 
#### Check these options or Enable them :
* windows hypervison platform
* windows projected file system
* windows subsystem for linux
* virtual machine platform
### OR
#### 1. Open PowerShell as Administrator (Start menu > PowerShell > right-click > Run as Administrator) 
### or 
#### Press ```Win``` + ```X``` and select Windows Terminal (Admin) or PowerShell (Admin).

## Step 2: Enable ```optionalfeature``` using command line. (You can skip this)
####  If somehow any feature is Disable or missing just run these commands It going to Re-Enable them. 
```bash
 dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestar
```
```bash
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

## Step 3: Download the Linux kernel update package.

#### Tap on link, It will Directly download the kernal of x64. 

#### [Wsl Linux kernal](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)

#### Open Poweshell as Administrator Past this:
```bash
wsl.exe --install or wsl.exe --update
```
```bash
wsl --set-default-version 2
```

## Step 4: Download Distro of Your Choice.
#### Go to Microsoft store search and download distro according to you.
# <div align="center"><img src= https://miro.medium.com/max/4510/1*ZL4F03VmPm-qQR6mdbto2Q.png align="center" width="600" ></img></div>
## Step 5: Config Distro
#### Open downloaded distro 
#### Creat user & pass for your distro
#### Run following commands to update and upgrade.
```bash
sudo apt-get update -y && sudo apt-get upgrade
```
### To Install REMOTE DESKTOP (Note : It didnt work with ever dirstro, but work with few like Kali)
```bash
sudo apt install kali-desktop-xfce -y
```
```bash
sudo apt install xrdp -y
```
```bash
sudo service xrdp start
```
### To Start Remote desktop type ```Kex``` on terminal.
```bash
kex
```
### 🙂


