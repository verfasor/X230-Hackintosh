[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/mighil)

**DISCLAIMER: YOU'RE NOTHING BUT AN A-HOLE IF YOU SELL EFI FOLDER (CONFIG) THAT'S ALREADY AVAILABLE FOR FREE OF COST. DON'T DO THAT.**

# X230 Hackintosh Catalina Clover & Config.

Fork or star, it's your call.

![X230 from 2012 Living The Catalina Dream!](https://i.redd.it/srs2yme8sgr31.jpg)

EFI Folder (Clover), plist, and BOOT required to install/run Thinkpad X230 Hackintosh Catalina 10.15. Files are from [@littlegtplr](https://github.com/littlegtplr/Hackintosh-X230-macOS). Move these files to your EFI Folder. I've got another EFI folder labelled **EFI-test**. Feel free to tinker that also. 

# #README

- Proceed with caution.
- Kindly delete the RtWlanU & RtWlanU1827 kexts from **kexts/Other** folder.
- N/A for Opencore bootloader. Go ahead though, if you know what you're doing. 
- EFI-swap recommended. I haven't tested these settings against the latest version of Clover.

I added [Realtek WLAN kexts](https://github.com/chris1111/Wireless-USB-Adapter-Clover) to use with the Comfast USB Wi-Fi adapter. You should edit the config. according to your preferences. 

The EFI folder is applicable for Vanilla approach and SSD hot-swap (just replace/paste EFI folder - not recommended though.) 

# What Doesn’t Work?

- Inbuilt WiFi, you can hack BIOS/install a Mac-compatible WiFi card. I highly recommend an external device like Comfast CF-811AC for the time being.
- Fingerprint reader

# FAQ. 

- [Please visit this reddit thread](https://www.reddit.com/r/hackintosh/comments/dfdf3l/x230_from_2012_living_the_catalina_dream/).
- I've used [neofetch](https://github.com/dylanaraps/neofetch) to display system specs via Terminal.

# TMI

I sell modded ThinkPad X230s. I'm an expat in China, and I've connections with ThinkPad enthusiasts here. We can ship modded X230 machines (1080p mod, 2k mod, Quad code CPU mod, and more) to any country. Email **mighil@pm.me**. or use the email ID in my bio.

# A better screenshot

![https://i.redd.it/6rq528gjtgr31.png](https://i.redd.it/6rq528gjtgr31.png)

# How to create a bootable macOS Catalina 10.15 USB install drive? (on MacOS)

[Refer to this guide from 9to5mac](https://9to5mac.com/2019/06/27/how-to-create-a-bootable-macos-catalina-10-15-usb-install-drive-video/)

# How to create a bootable macOS Catalina 10.15 USB install drive? (on Windows)

1. Install [Transmac](https://www.acutesystems.com/scrtm.htm) on a Windows machine. It has a 15-day trial period and works flawlessly flashing DMG files to USB.

2. Download the [MacOS 10.15 with clover dmg file from here](https://mirrors.dtops.cc/iso/MacOS/daliansky_macos/) or other sources you come across Google SERP.

3. Download the EFI folder from this repo.

4. Download [Clover Configurator for macOS](https://mackie100projects.altervista.org/download-clover-configurator/) (latest version).

5. Connect a 16 GB USB flash drive.

6. Open Transmac. In the left pane, right-click the USB Drive and select Format Disk for Mac

7. Again in the left pane, right-click the USB Drive and select Restore with Disk Image. Then select the DMG file I mentioned in (2). Flashing process will take a few minutes depending on the size of .dmg and speed/port of the USB drive.

8. Install [DiskGenius](https://www.diskgenius.com/).

9. Locate the USB drive in DiskGenius. Delete the EFI folder and replace it with the new EFI folder. 

10. Plug the USB drive into the X230 and boot from USB.

11. Format the disk drive to APFS, install macOS Catalina, and restart the system.

12. Connect Hackintosh system to the Internet via LAN cable, USD tethering or a Mac-compatible external WiFi adapter.

13. Download & install Clover Configurator on MacOS. Open EFI partition and copy -> paste the the EFI folder once more. 

14. You may use [Karabiner-Elements](https://pqrs.org/osx/karabiner/) if the keyboard mappings (command and option) are acting up.

All the best.
