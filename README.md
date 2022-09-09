# ![alt text](https://cdn.discordapp.com/attachments/936755058626928735/1017882711089754223/app_wireframe_1.png)
Repository for UF CpE Design project,  uControl, the universal Bluetooth game controller adapter. 

# Contributors
* Andres Maldonado-Martin
* Mason Anderson
* Juan Pablo Lancheros
* Sam Fleischer

# Stakeholders
* TA: Evan Rocha

# Project Description
uControl is a all-in-one wireless game controller emulator, allowing you to pair controllers to your PC and emulating controller inputs. Using the uControl Companion App, you are able to manage the devices that are connected to the uControl module and select which (if any) emulation you want, allowing users to have quality emulated controllers for consoles they do not own, all while reducing the need for external input emulators such as XInput, and combining them into a single, wireless package. Using a PS2 emulator but don't have a PS2 controller? uControl will solve all these issues with a single product.

Use the uControl Companion App:
* Make sure your uControl is plugged in and has adequate power.
* Launch the uControl Companion App.
* For first time setups, click "Scan for uControl".
* Once the uControl device has been found, click "Change Controller".
* Select the controller type you are trying to pair with (Nintendo Switch/Playstation/Xbox/Phone)
* Click the back button to "Change Console".
* Select the controller input emulation of your choice (Nintendo Switch/Playstation/Xbox).
* Send the configuration to the uControl using the "Send Configuration" button.

# Schematics and Diagrams


# Build Instructions
## Firmware: (ATXMEGA128A1U)
Must have Microchip studio installed along with the AVR device support that comes with the installation of Microchip studio.
Download and open the Atmel Solution file in the Microchip branch.
Under Tools>Device make sure to select the XMEGA plugged into a USB slot on your computer.
If you do not have an XMEGA, you can test the build by selecting "Simulator" as your device.
Press the run button and the code will automatically be uploaded to the XMEGA.

## Companion App: (Android Device running Android 11 or lower)
Ensure you have developer mode enabled on your device.  Perform either of the following:
* (RECOMMENDED) Install .apk file located at the root of this repository directly onto your Android device.  You may need to allow unknown apps in Settings.
* Install Android Studio on your computer.  Create a new project from Version Control (VSC) and clone it from this repository.  Plug your Android device into your computer via USB.  If Android Studio doesn't recognize your phone you must enable USB Debugging in the Developer Settings on your device.  Build the project and then select your plugged in Android device as the target device.  Hit the Run button and it should install the application and run it on your device.
