## Introduction

Creating a dynamic script to remove bloatware across multiple computers for small to large business to free up RAM, reclaim storage space, and improve the overall speed and longevity of your PC.


## [Bloatware](https://www.techtarget.com/searchsecurity/answer/How-can-we-detect-and-uninstall-bloatware)
Bloatware is term to identify preinstalled packages onto your computer that is not needed. One example is the Bing Application that comes preinstalled with any windows 11 computer.


## [Get-AppxProvisionedPackage](https://learn.microsoft.com/en-us/powershell/module/dism/get-appxprovisionedpackage?view=windowsserver2025-ps)

The <b>Get-AppxProvisionedPackage</b> cmdlet gets information about app packages (.appx) in an image that are set to install for each new user. For information about app packages (.appx) that are not provisioned, use the Get-AppxPackage cmdlet instead.

In shorter detail - The package is installed on windows and will be installed for all future users. When you remove something, it will be removed for all users. 


#### Provision Packages by Organized Grid View (ogv)
![alt text](https://github.com/JeanPCQ/Remove_Bloatware/blob/main/Pic/Get-AppxProvisioned_ogv.png)

#### Provision Package Search
![alt text](https://github.com/JeanPCQ/Remove_Bloatware/blob/main/Pic/Get-AppxProvisioned_search.png)

#### Removing Provision Package
![alt text](https://github.com/JeanPCQ/Remove_Bloatware/blob/main/Pic/Get-AppxProvisioned_Removed.png)




## [Get-AppxPackage](https://learn.microsoft.com/en-us/powershell/module/appx/get-appxpackage?view=windowsserver2025-ps)
The <b>Get-AppxPackage</b> cmdlet gets a list of the app packages that are installed in a user profile. An app package has an .msix or .appx file extension. To get the list of packages for a user profile other than the profile for the current user, you must run this command with administrator permissions.

In shorter detail - The application is installed on the users end. If uninstalled, you are only uninstalling from that specifci user. 
