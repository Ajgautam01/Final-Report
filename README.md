# Week 1 Installation Ubuntu

1.   **Download Ubuntu** You can download the latest version of the Ubuntu desktop iso image from the Ubuntu website.(https://ubuntu.com/download/desktop)
2.  **Create a bootable USB disk :** Use Universal USB Installer (BIOS compatible) or Rufus [(UEFI compatible)http://rufus.ie/en/] to make a bootable USB disk
3.  **Boot from bootable USB :** Power on your system and press the ESC, F2, F10, F12, or DEL key to select the boot order.

Then, you need to select boot from USB or removable drive and to boot from USB.

4.  **Preparing to Install Ubuntu :** Ubuntu image will begin to load. Do not interrupt the booting of the Ubuntu image.When the system is completely booted from Live USB, you will get the OS installer that looks like below.

To install Ubuntu, click on the Install Ubuntu button.
Choose your keyboard layout. In case, if you don't know about your keyboard layout, use the Detect Keyboard Layout option. 

5.  **Normal/Minimal Installation :** On this screen, you need to pick the applications for installation.

*Normal Installation -* You will get a graphical desktop with all standard software.

*Minimal Installation -* You will get a basic desktop with an internet browser and core system utilities.

You can either decide to install updates and other third-party software while installing Ubuntu or leave it (you can install them later if you need).

The updates and third-party software installation requires a functioning internet connection with your system. The installation may take somewhat additional time relies on the downloadable contents.

For this demo, I decided to do the Ubuntu Normal installation.

6.  **Create Partitions :** At this point, if you have an empty hard disk then you will get only two options in the installation type. If you have installed other OS already in your system then you will get more options accordingly.

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

# Week 2 Android Studio

### Installation Guide of Gladiater Project

*Installation of Android studio*
* step - sudo apt install snapd
* step - Enter your password
* step - sudo snap install android-studio --classic
for uninstall of android studio - sudo snap remove android-studio

*Setup of Android Studio*
* Dialog Box - Help improve android studio - its your wish accept or reject.
* Next
* Choose standard and next
* Choose your theme
* Verify Setting - next
* License Agreement - Accept - next
* Downloading Components and Finish

*Setting android studio for Gladiater project*
* Open android studio and open project 
* Choose your project and enable Tick trust projects and click on trust project
* Automatically downloaded some files in android studio
* In Dialog box , they show some required files to downlaod -
     JavaSDK
     Android Gradle Plugin (upgrade recommendation)
* Sync Project with Gradle Files
* Go on SDK Manager and download suitable versions of android then apply and download it.
* Now on SDK Manager - Go on tools and download NDK(Side by Side).
* Restart your Android studio
* Connect your android device with usb cable and make sure your usb debugginng is on. Then choose your device and click on Build Project. Now its takes some time and app is now available to run in your phone.

## First Basic App *unit Converter*
 follow  Code with Harry Android Studio Tutorial on YOUTUBE  for making First Basic App Unit Converter.
 The working of unit converter is convert number into Pounds.
 
 # Week 3 Flutter & Dart 
 ## Flutter
  Flutter provides basic and advanced concepts of the Flutter framework. Flutter is a UI toolkit for building fast, beautiful, natively compiled applications for mobile, web, and desktop with one programing language and single codebase. It is free and open-source. Initially, it was developed from Google and now manages by an ECMA standard. Flutter apps use Dart programming language for creating an app.
 
 In general, creating a mobile application is a very complex and challenging task. There are many frameworks available, which provide excellent features to develop mobile applications. For developing mobile apps, Android provides a native framework based on Java and Kotlin language, while iOS provides a framework based on Objective-C/Swift language. Thus, we need two different languages and frameworks to develop applications for both OS. Today, to overcome form this complexity, there are several frameworks have introduced that support both OS along with desktop apps. These types of the framework are known as cross-platform development tools.
 
 ## Dart
 The Dart language is type safe; it uses static type checking to ensure that a variable’s value always matches the variable’s static type. Sometimes, this is referred to as sound typing. Although types are mandatory, type annotations are optional because of type inference. The Dart typing system is also flexible, allowing the use of a dynamic type combined with runtime checks, which can be useful during experimentation or for code that needs to be especially dynamic.
 
 Get the Flutter SDK
Download the following installation bundle to get the latest stable release of the Flutter SDK:


For other release channels, and older builds, see the SDK releases page.

Extract the zip file and place the contained flutter in the desired installation location for the Flutter SDK (for example, C:\src\flutter).
If you don’t want to install a fixed version of the installation bundle, you can skip steps 1 and 2. Instead, get the source code from the Flutter repo on GitHub, and change branches or tags as needed. For example:
git clone https://github.com/flutter/flutter.git -b stable

## Update your path
If you wish to run Flutter commands in the regular Windows console, take these steps to add Flutter to the PATH environment variable:

* From the Start search bar, enter ‘env’ and select Edit environment variables for your account.
* Under User variables check if there is an entry called Path:
* If the entry exists, append the full path to flutter\bin using ; as a separator from existing values.
* If the entry doesn’t exist, create a new user variable named Path with the full path to flutter\bin as its value.
You have to close and reopen any existing console windows for these changes to take effect.

## Run flutter doctor
From a console window that has the Flutter directory in the path (see above), run the following command to see if there are any platform dependencies you need to complete the setup (C:\src\flutter>flutter doctor).This command checks your environment and displays a report of the status of your Flutter installation. Check the output carefully for other software you might need to install or further tasks to perform (shown in bold text).

# Week 4 Set up an  Flutter editor
You can build apps with Flutter using any text editor combined with Flutter’s command-line tools. However, we recommend using one of our editor plugins for an even better experience. These plugins provide you with code completion, syntax highlighting, widget editing assists, run & debug support, and more.

Use the following steps to add an editor plugin for VS Code, Android Studio, IntelliJ, or Emacs. If you want to use a different editor, that’s OK, skip ahead to the next step: Test drive.
## Install VS Code
VS Code is a lightweight editor with complete Flutter app execution and debug support.

VS Code, latest stable version

## Install the Flutter and Dart plugins
Start VS Code.
Invoke View > Command Palette….
Type “install”, and select Extensions: Install Extensions.
Type “flutter” in the extensions search field, select Flutter in the list, and click Install. This also installs the required Dart plugin.

Validate your setup with the Flutter Doctor
Invoke View > Command Palette….
Type “doctor”, and select the Flutter: Run Flutter Doctor.
Review the output in the OUTPUT pane for any issues. Make sure to select Flutter from the dropdown in the different Output Options.

## Test drive
To create a new Flutter app from templates, run it, and experience “hot reload” after you make changes to the app.

Select your development tool of choice for writing, building, and running Flutter apps.
## Create the app
* Invoke View > Command Palette.
* Type “flutter”, and select the Flutter: New Project.
* Select Application.
* Create or select the parent directory for the new project folder.
* Enter a project name, such as my_app, and press Enter.
* Wait for project creation to complete and the main.dart file to appear.

The above commands create a Flutter project directory called my_app that contains a simple demo app that uses Material Components.

# Week 5 First app in Flutter 
Create the starter Flutter app

Create a simple, templated Flutter app, using the instructions in Getting Started with your first Flutter app. Name the project startup_namer (instead of flutter_app).
You’ll mostly edit lib/main.dart, where the Dart code lives.

1. Replace the contents of lib/main.dart.
Delete all of the code from lib/main.dart. Replace with the following code, which displays “Hello World” in the center of the screen.
2. Run the app in the way your IDE describes. You should see either Android, iOS, Windows, Linux, macOS, or web output, depending on your chosen device.

 # Week  Python 
 Do task in django python
* Function
* String
* Algorithms
* Linear or Non-linear Equation
 
 # Week  Python 
 Do task in django python
 * Tuples
 * Loops
 
  # Week  Python 
 Doing Backend django python Assingment
 
 # Week 6 install nodejs and React
 ### Follow Installation Guide of nodejs or npm and rect in Ubuntu 
 watching React tutorial of code with Harry on YOUTUBE
 
 
 
 
 # Week UI/UX
 follow UI/UX(Figma) tutorial on YOUTUBE for making blueprint
 
  
 
 # Week  UI/UX 
   Work on Figma for making blueprint of Android app. The aim of blueprint is to make a  better app or reduce work load
 
 



