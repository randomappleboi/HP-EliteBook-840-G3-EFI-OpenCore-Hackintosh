# HP EliteBook 840 G3 EFI  

## Opencore EFI folder for HP ELiteBook 840 G3  

![Screenshot](https://raw.githubusercontent.com/randomappleboi/HP-EliteBook-840-G3-EFI/refs/heads/main/Sequoia.png)

macOS Sequoia 15.0 final beta
   
   
**Warnings:**  

This might not work for your computer. Please check compatibility with your laptop using my specifications listed below. No garuantee. If you seek support, please DM me on [Reddit](https://reddit.com/u/randomappleboix). Also, you'll need to to populate the SMBIOS yourself. Please refer to the SMBIOS part of this document.

**What works and what doesn´t**

 - Working:
     - Trackpad
     - Keyboard
     - Bluetooth
     - Speakers
     - Display port
     - SD card reader
     - Webcam
     - Most other ports (unable to test: big card reader, SIM slot)
     - Basically everything else
     - Native Wifi (you *need* to follow my guide linked **here**, *or* use heliport and disable the native symbol in Settings > Control Center)

 - Not working:
     - Display out via Dock (USB via Dock works)
     - yet to be dicovered

 - Notes:
     - Airdrop works from MacBook to iPhone, not the other way around (only after using my **tutorial**, not with heliport)

**SMBIOS**

You have to fill in the SMBIOS information yourself. This means giving your MacBook a serial number, amongst other things. Don't worry, it's super easy.

1. Download [ProperTree](https://github.com/corpnewt/ProperTree) or OCAT to edit your config.plist. Open the config.plist located under EFI > OC.
2. Download [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) and open it in terminal.




**Specs**

 - HP EliteBook 840 G3  
 - Intel Core i5 6300U  
 - Intel HD Graphics 520  
 - Synaptics touchpad  
 - 1080p LCD 14" (no touch)  
 - Intel AC 8260 Wireless card
 - 500GB Samsung SATA SSD

**EFI**

 - Opencore 1.0.3
 - All kext (at least all important ones) are updated to their latest version.
 - If you have more time than me and want to further improve this project, feel free to do so. Also, you can DM me your edit or recommendations and I will publish the changes on this repository.
 - I don´t have all that much time, but I will try to always keep this updated.
 - **Do not redistribute without my explicit permission!**

**Other important stuff**

 - You will have to modify you bios settings, please refer to [Dortania´s Guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/skylake.html#intel-bios-settings) for that.
 - You will also have to install macOS to a USB, refer to [this part of Dortania´s guide](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/windows-install.html) for that.
 - When troubleshooting, refer to [Dortania´s troubleshooting section](https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/troubleshooting.html) or to the [Hackintosh subreddit](https://reddit.com/r/hackintosh)
 - Wifi doesn´t work and never will natively, you have to use ethernet for the installation, then download [Heliport](https://github.com/OpenIntelWireless/HeliPort/releases/tag/v1.5.0) and add it to the login applications.
 - Tested on Sonoma 14.4.1 and 15.0 final beta.
 - When using a NVMe drive you might have to manually add [NVMefix.kext](https://github.com/acidanthera/NVMeFix/releases)

**Legacy Screenshots:**

![Screenshot](https://github.com/randomappleboi/HP-EliteBook-840-G3-EFI/blob/main/Sonoma.png)

macOS Sonoma 14.4.1

