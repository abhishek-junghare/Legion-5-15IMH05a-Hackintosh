# Legion 5 15IMH05a - Hackintosh Big Sur (Dual Boot - Same Drive)

## Dual boot macOS Big Sur & Windows on same drive
Intel Core i5 10300H + nVidia GTX 1650 4GB

> You will be responsible for any loss or damage whatsoever caused. Taking a backup is recommended.

## Guides
* (Main Guide) Dortania's OpenCore Installation Guide - [View Guide](https://dortania.github.io/OpenCore-Install-Guide/)
* MacOS Installation & Post Installation Steps (Video Guide for Additional Reference) - [View Guide](https://youtu.be/IP7crXa-5lo?t=180)
* Dual Boot Hackinotosh Guide by Brandon Yen - [View Guide](https://youtu.be/ztxHRGdX0Sw)

## Steps to Follow

> BIOS Settings: F2

> Boot Menu: F12

### 1. Install macOS

* Make a macOS Installer USB - [View Guide](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/winblows-install.html)
* [Download EFI](https://github.com/abhishek110022/Legion-5-15IMH05a-EFI/releases) and place the EFI folder it in macOS Installer USB - [Reference Screenshot](https://dortania.github.io/OpenCore-Install-Guide/assets/img/com-efi-done.a6fb730e.png)
* Disable 'Secure Boot' from BIOS Settings
* Boot from the Installer USB (Will be named as 'EFI USB Device')
* Install macOS (Erasing the drive will remove everything on that drive, take a backup first) - [View Guide](https://youtu.be/IP7crXa-5lo?t=196)
* If everything works properly, then move OpenCore from USB to macOS Disk - [View Guide](https://dortania.github.io/OpenCore-Post-Install/universal/oc2hdd.html)
* Post Installation (if required) - [View Steps](https://dortania.github.io/OpenCore-Post-Install/)

### 2. Install Windows 10 (Same Drive)

* Make a Windows Installer USB
  - Download [Windows 10.iso](https://www.microsoft.com/en-in/software-download/windows10ISO)
  - Format USB Drive as exFAT (Master Boot Record) from macOS Disk Utility
  - Open Windows 10 ISO file and copy all the content to the formatted USB Drive
* Follow the [Dual Boot Guide](https://youtu.be/ztxHRGdX0Sw)

## Not Working :(
* HDMI
* Black screen after sleep (disable sleep & set 'Turn display off' to never from macos)

## Credits
* Thanks to [@LuckyCrack](https://github.com/LuckyCrack) for base EFI - https://github.com/LuckyCrack/Legion-5i-EFI
* Thanks to [@dortania](https://github.com/dortania) for OpenCore Guide
