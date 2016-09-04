# Setting-up-Linux
## Description
The sets I have taken to setup linux on my laptop.  They are mainly here to help me remember the exact commands that were required to either install new 'items' or fix problems.

## To get something installed
* (Obvious) Download the iso for the desired distro.  ie Ubuntu
* Download rufus from [Here](https://rufus.akeo.ie/).  This helps creating a bootable USB stick with the downloaded ISO.
* Boot from the USB in the computer.  
  * During the install, I chose to use UFI as the loader(?).  This has cause the BIOS's boot device selector at each power up.  

## First boot
* Find a Terminal and run:
  * `sudo apt-get update`
  * `sudo apt-get upgrade`
* Install Graphics(Works for Nvidia)
  * `sudo add-apt-repository ppa:graphics-drivers/ppa`
  * `sudo apt-get update`
  * `sudo ubuntu-drivers autoinstall`
  * `sudo reboot`
  * Noted after this the boot process took longer, don't know why

## Installing Virtual Box 
* Download VirtualBox from [Here](https://www.virtualbox.org/wiki/Linux_Downloads)
* Will also need the extension, get it [Here](https://www.virtualbox.org/wiki/Downloads)
  * The extension pack is need to pass though USB2 and USB3.  I'm sure there is other things it is good for.

## If there is funny mouse artifacts/echos or what ever still hanging around.  This can be improved be changing the display settings.
* System Settings > Display > Compositor
  * You can try changing "Tearing Prevention(vsync)" to full screen repaints, but 'they' say it is more hardware intentsive.
  * The other option is to turn off OpenGL and use XRender.
* OpenGL requires an installed graphics card to render the screen.  Where as XRender is an extension of XServer and does not required graphics.  XRender also doesn't support as many features compared to OpenGL, it is simple and basic.  Explained better [here](http://stackoverflow.com/questions/22318322/what-is-the-difference-between-opengl-and-xrender-in-kde-desktop-effects)

## Next  