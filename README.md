**# Week 1 Installation Ubuntu and Android Studio **

1.   **Download Ubuntu** You can download the latest version of the Ubuntu desktop iso image from the Ubuntu website.(https://ubuntu.com/download/desktop)
2.  **Create a bootable USB disk :** Use Universal USB Installer (BIOS compatible) or Rufus (UEFI compatible) to make a bootable USB disk
3.  **Boot from bootable USB :** Power on your system and press the ESC, F2, F10, F12, or DEL key to select the boot order.

Then, you need to select boot from USB or removable drive and to boot from USB.
4.**Preparing to Install Ubuntu :** Ubuntu image will begin to load. Do not interrupt the booting of the Ubuntu image.When the system is completely booted from Live USB, you will get the OS installer that looks like below.

To install Ubuntu, click on the Install Ubuntu button.
Choose your keyboard layout. In case, if you don't know about your keyboard layout, use the Detect Keyboard Layout option. 
5.  **Normal/Minimal Installation :** On this screen, you need to pick the applications for installation.

*Normal Installation -* You will get a graphical desktop with all standard software.

*Minimal Installation -* You will get a basic desktop with an internet browser and core system utilities.

You can either decide to install updates and other third-party software while installing Ubuntu or leave it (you can install them later if you need).

The updates and third-party software installation requires a functioning internet connection with your system. The installation may take somewhat additional time relies on the downloadable contents.

For this demo, I decided to do the Ubuntu Normal installation.

6.  Create Partitions

At this point, if you have an empty hard disk then you will get only two options in the installation type. If you have installed other OS already in your system then you will get more options accordingly.

Because we want to set up partitions manually so choose Something else and click Continue.
on this screen, the installer will list all the accessible hard disks.

Since this is the new disk, I needed to click on New Partition Table to make an empty partition.
Next, click Continue from the pop-up window to make an empty partition table on the system.
We will now create four partitions for our Ubuntu installation.

*- These Partitions are:*

/boot

swap

/home

/ -- (root)

Select the free space and afterward click on the + sign at the bottom left to make a partition.

The following image shows for /boot partition.
The following screen shows the swap partition. The swap partition serves as an overflow space for your RAM. If your RAM fills up totally, any extra applications will run off the swap partition rather than RAM.

It is recommended to have the swap partition double the size of the RAM. And I also recommend never create a swap partition of more than 4GB.

Here, I have created a 4GB swap partition. If your system has enough memory, then you can choose not to have a swap partition.
The following is for /home partition.
We will use the remaining space for the / (root) partition.
Review your partition layout and click on **Install Now** button.
Click on the **Continue** button to create partitions as per the plan.

7.  **Additional Configurations:** On the next screen, select your timezone location from the map. Then, click on the Continue button.
                                    On this screen, you can create a username and password to get access to your system.

Additionally, set the hostname for your system.

Here is one thing you should remember - if you chose to log in automatically, then the system will directly take you to the desktop without asking for any credentials.

Click on Continue.
On this screen, you can create a username and password to get access to your system.

Additionally, set the hostname for your system.

Here is one thing you should remember - if you chose to log in automatically, then the system will directly take you to the desktop without asking for any credentials.

Click on **Continue.**
The installation will take near about 10 to 15 minutes. Once the installation is complete, **restart** your machine.

When the system is restarted, you will get a login window. Sign in to your system with the username and password that you created earlier.



