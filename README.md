# Wsl  Linux
### Install Your favourate distro on Windows 11
### Install linux windows subsystem for linux (wsl) on windows 11 ,Linux on windows terminal run Operating system such as kali linux , Ubuntu , Arch.

 # W S L _ L i n u x _ I n s t a l l 


# Step 1:

## Press => window + R key On Keyboard typer ```optionalfeature``` 
## Scroll down and and check this option or enable them :- 
* windows hypervison platform
* windows projected file system
* windows subsystem for linux
* virtual machine platform

  
# Step 2:

## Open PowerShell as Administrator (Start menu > PowerShell > right-click > Run as Administrator)

# Step 3:   ----- enter this command ------
### To enable feature by somehow any biggner can miss or maybe it gonna dissable by any chance

```bash
 dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestar
```
```bash
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```


# Step 4:        ----- Download the Linux kernel update package -----

## Tap on link It Directly download it 

## [Wsl Linux kernal](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)

# Open Poweshell as Administrator Past this
```bash
wsl.exe --install or wsl.exe --update
```
```bash
wsl --set-default-version 2
```

# Step 5:
## Open Microsoft store search and download distro of ur choice
![Screenshot 2024-04-27 020128](https://github.com/Esther7171/Wsl-kali/assets/122229257/df78ae70-6c30-4fe5-a5e6-e7d8f03834d3)

# Step 6:
## Open download distro 
### creat user pass for your distr
## Run following commands
```bash
sudo apt-get update -y && sudo apt-get upgrade
```
# TO Install REMOTE DESKTOP
```bash
sudo apt install kali-desktop-xfce -y
```
```bash
sudo apt install xrdp -y
```
```bash
sudo service xrdp start
```
```bash
kex
```
