## Pre-workshop Setup (Must be completed in advance of the HOL)

Please perform the following steps in advance of the Hands-on-labs otherwise you will spend a significant time during the workshop performing these steps.

### Raspberry Pi Setup

You will need to walk through the following steps on your Raspberry Pi prior to the hands-on-lab. <BR>

1. Ensure your Raspberry Pi can boot [Raspian] (https://www.raspberrypi.org/downloads/) from the SD card. 
  - Follow the instructions to install the operating system: [NOOBS] (https://www.raspberrypi.org/downloads/noobs/) 
  - If you have a new microSD card that hasn't been formatted before, use [SDFormatter](https://www.sdcard.org/downloads/formatter_4/eula_windows/) to do a full format of the card.
  - Insert the microSD card into your Pi and connect the power supply. 
  - Click to install Raspbian
     <p align="center">
        <img src="Images/NOOBS_Install.jpg" width="50%" height="50%"/>
      </p>
   - Confirm the deletion of content on the SD card and the installation of the OS. 
      <p align="center">
        <img src="Images/ConfirmInstall.jpg" width="50%" height="50%"/>
      </p>
2. If you do not have the Sense HAT and will be using the Sense HAT Emulator, you will have to run through some extra steps to ensure that you access the Sense HAT Emulator graphically: 
  - First, run through the steps to ensure it's installed. Verify by checking under 'Programming' in the Raspian GUI.

      <p align="center">
        <img src="Images/SenseHat.jpg"  width="50%" height="50%"/>
      </p>
      
   - Next, make sure that VNC is enabled. We will be using VNC so that a physical monitor will not be required for the labs. 
     - Select Menu -> Preferences -> Raspberry Pi Configuration -> Interfaces.
     
        <p align="center">
          <img src="/images/menu.jpg"  width="50%" height="50%"/>
        </p>
        
     - Ensure VNC is Enabled.
     
        <p align="center">
          <img src="/images/enableVNC.jpg"  width="50%" height="50%"/>
        </p>
         
3. Enable SSH on the Raspberry Pi. You will be SSH-ing to the Raspberry Pi to modify and execute scripts. 
  
  - In the menu, choose "Preferences", then "Raspberry Pi Configuration"
  - Enable SSH

### Laptop Setup

The following steps will walk you through the installation of tools that you need to run on your laptop for this lab: 

1. Install [Device Explorer](https://github.com/Azure/azure-iot-sdk-csharp/releases/download/2017-8-10/SetupDeviceExplorer.msi) on your Windows laptop. Device Explorer is a great tool that can be used to perform operations such as manage the devices registered to an IoT hub, view device-to-cloud messages sent to an IoT hub, and send cloud-to-device messages from an IoT hub. Documentation for Device Explorer can be found [here](https://github.com/Azure/azure-iot-sdk-csharp/tree/master/tools/DeviceExplorer) <BR>
If you are running a non-Windows machine, device explorer will not work and you will need to use the command-line tool - iothub-explorer. The instructions for on how to install and use iothub-explorer is [here](https://github.com/azure/iothub-explorer)
2. Download and install [PuTTY](http://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html). We will use PuTTY to SSH into the Raspberry Pi to perform various functions throughout the lab. 
3. If you are using the Sense HAT Emulator (vs the physical device), you'll need to install VNC viewer on your laptop so that you can remotely view your Raspbian desktop. Download and install RealVNC from (https://www.realvnc.com/download/viewer/)
4. Ensure your Azure subscription login is working and you have sufficient permissions to create resources.

