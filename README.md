# CUNY Tech Prep: Pre-orientation setup

On June 27th, 28th, and 29th we will be holding orientation sessions for the CTP cohort 3 students. (Note, you only need to come into one session, all three days will cover the same materials). During orientation we will provide you an overview of the program and answer any questions you may have. In addition, we will use some of that time to setting up your development environment. The instructions below will provide you information on what to download and install prior to the orientation session. You should complete as much of this as you can on your own, if at any point you get stuck, document how much you completed and what your errors were, and we will help you complete setup during the orientation session.


## Github Account Setup

Prior to orientation, make sure you have an active Github account. Verify that you know your github username and password, and are able to login.

## Development Environment Setup

In this program we will be developing web applications in JavaScript using Node.js. While Node.js has installers available for Windows, Linux, and MacOS, our previous experience shows that Node.js development on Windows is very buggy and often complicated. Therefore, our program will not provide support for Windows users and we encourage you to try Linux instead, for installation you have two options outlined below in the Windows Users section. For Linux and MacOS users, see the notes below for your current operating system to decide which environment you want to work in.

### Linux Users

If you are already a Linux Operating System user, then I will assume you know what you are doing :) The only things you should work on prior to orientation is making sure your operating system is up to date, and that you have a working text editor that works with JavaScript.

For your reference, our program staff will be using Lubuntu (an Ubuntu 16.04 (64bit) based distribution with students new to Linux). If you used a non Ubuntu based distribution, make sure you are familiar with your package manager.

### MacOS Users

If you are using MacOS then you can either develop directly on the Mac or you can choose to install the Linux Virtual Machine. If you opt to develop directly on the Mac, then make sure you have applied all security updates, installed the latest version of XCode, and you should install/update Homebrew [https://brew.sh/](https://brew.sh/). And make sure you are familiar with launching your terminal.

Homebrew is a package manager for the MacOS which makes the installation of software packages very easy, I highly recommend it.

### Windows Users

Since we wont be supporting Windows development, we encourage you to take this opportunity to try out a Linux based Operating System. You have two options for getting Linux running on your computer

**Dual Booting** NOTE: THIS IS RISKY. ONLY ATTEMPT IF YOU HAVE YOUR DATA BACKED UP RELIABLY. If you are familiar with disk partioning and installing multiple operating systems, then you can dual boot your computer to run both Linux and Windows. Dual booting can sometimes lead to all data loss. CTP staff will not be able to help you with this setup. If you still opt to go this route then we recommend the Ubuntu 16.04 LTS distribution.

**Virtual Machine** The second option will install a Linux Virtual Machine that runs within Windows. This is less risky than the Dual Booting option. Instructions are in the next section.


## Setting up a Linux Virtual Machine

If you have opted to install a Linux Virtual Machine, use the following instructions.
 
### Download the following:

- VirtualBox 5.1.22 [https://www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads)
  + Download the version for your current Operating System.
- Lubuntu 16.04.2 [http://cdimage.ubuntu.com/lubuntu/releases/16.04/release/lubuntu-16.04.2-desktop-amd64.iso](http://cdimage.ubuntu.com/lubuntu/releases/16.04/release/lubuntu-16.04.2-desktop-amd64.iso)
  + Lubuntu is an Ubuntu based distribution. The only reason Lubuntu was chosen is because it uses less RAM and Disk than the standard Ubuntu distribution. If you have a preference for another Ubuntu 16.04 based distribution, go for it.

### Install VirtualBox

- Double click on the installer
- Perform a Standard Install (with default selections)

### Create a Virtual Machine (VM)

Launch VirtualBox. Click on the "New" button on the upper left corner of the window. Provide the Virtual Machine a Name, and select the Type and Version to match the following image.

![create-virtual-machine.png]

Next, you will be asked to select an amount of Memory. 1024 MB should be the minimum you select. If your computer has more than 4GB of memory or you know what you are doing, then you can increase this amount.

![select-memory.png]

Next, you will be asked about the Hard disk, select "Create a virtual hard disk now", click "Create",

![select-harddisk.png]

then select the "VDI" option, then the "Dynamically Allocated" option, then you will be asked how much space to assign the hard disk. 10GB is the minimum you should choose. You can assign more space (20-40GB) if you plan on using this virtual machine for additional development and if you have the space available on your computer.

The Virtual Machine is now ready to be booted for the first time.

### Installing Lubuntu

In VirtualBox, select the VM you just created, and press the "Start" button.

The first time you start the VM, it will ask you for the location of the OS disk. You can click on the folder and select the Lubuntu `.iso` file you previously downloaded, then press "Start".

![select-lubuntu-iso.png]

You will now be presented with the Lubuntu installation menu. You can leave all the default options as they are if you don't know what they are for. Here is a list of the default options you should see:

- Select your language: English
- Select: "Erase disk and install Lubuntu"
- Continue (with default disk partitions)
- Select your Location
- Press enter on keyboard layout
- Provide your name and password (remember this, you'll need it in future)
![create-lubuntu-account.png]

The installation takes a few minutes to an hour depending on your computers specs. Once installation is done, Restart the VM.


### First time running VM

To verify that the installation went smoothly, make sure your computer has internet access and in the VM do the following:

- Login with your Username and Password
- Click on lower left corner menu
    * Select "System Tools" > "LXTerminal"
    * In the terminal, run the following:
        -  `sudo apt-get update`
        -  `sudo apt-get upgrade`
        -  This will take a few minutes, when completed, restart the VM

## You are now ready for the orientation session. 

Don't worry about installing Node.js and other software, we'll discuss it during orientation.

If you get stuck installing the Linux VM, don't worry. Just make sure that before coming into the orientation session you have already downloaded VirtualBox and Lubuntu.

See you at Orientation.




