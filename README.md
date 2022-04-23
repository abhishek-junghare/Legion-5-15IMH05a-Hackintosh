# Lenovo Legion 5 15IMH05a - EFI

> Disclaimer: You will be responsible for any loss or damage whatsoever caused. Taking a backup is recommended.

## Tested on Catalina 10.15.7 using OpenCore 0.8.0

## Guides
* (Main Guide) Dortania's OpenCore Installation Guide - [View Guide](https://dortania.github.io/OpenCore-Install-Guide/)
* MacOS Installation & Post Installation Steps (Video Guide for Additional Reference) - [View](https://youtu.be/IP7crXa-5lo?t=180)

## Specifications
* Intel i5 10300H
* GTX 1650 (Not Supported)

## Steps to Follow
* Make a macOS Installer USB - [View Guide](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/winblows-install.html)
* Download this EFI and place it in the root of USB - [Reference Screenshot](https://dortania.github.io/OpenCore-Install-Guide/assets/img/com-efi-done.a6fb730e.png)
* Disable 'Secure Boot' from BIOS (BIOS Key - F2)
* Boot from the Installer USB (Change Boot Order - 'EFI USB Device' at Top)
* Install macOS (Erasing the drive will remove everything on that drive, take a backup first) - [View Guide](https://youtu.be/IP7crXa-5lo?t=196)
* If everything works properly, then move OpenCore from USB to macOS Disk - [View Guide](https://dortania.github.io/OpenCore-Post-Install/universal/oc2hdd.html)
* Post Installation (if required) - [View Steps](https://dortania.github.io/OpenCore-Post-Install/)
  
## Not Working :(
* Trackpad
* HDMI

## Notes
* Use USB Tethering to share internet from your phone if WiFi is not working at the macOS installation step
* To access EFI after moving from USB to macOS Drive, use Terminal to mount EFI - [View Guide](https://hologos.github.io/how-to-mount-efi-from-command-line-terminal/)
* WiFi kext needs to be changed depending on macOS version - [Download WiFi Kext](https://github.com/OpenIntelWireless/itlwm/releases)
* config.plist needs to be updated after changing EFI contents like WiFi kext above. Use snapshot feature from ProperTree for updating - [Download ProperTree](https://github.com/corpnewt/ProperTree)
* In case the system doesn't boot properly after changing EFI contents or anything, just boot from the macOS Installer USB that we created before. Make the changes in the EFI from macOS Drive as required.
* Better to store the contents of the macOS Installer USB to your phone or cloud storage in case of any future use.
