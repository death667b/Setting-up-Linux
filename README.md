# Setting-up-Linux
## Description
The sets I have taken to setup linux on my laptop.  They are mainly here to help me remember the exact commands that were required to either install new 'items' or fix problems.

## To get something installed
* (Obvious) Download the iso for the desired distro.  ie Ubuntu
* Download `rufus`.  This helps creating a bootable USB stick with the downloaded ISO.
* Boot from the USB in the computer.  
* * During the install, I chose to use UFI as the loader(?).  This has cause the BIOS's boot device selector at each power up.  

## First boot
* Find a Terminal and run:
  * `sudo apt-get update`
  * `sudo apt-get upgrade`