[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/mighil) [![捐赠](https://img.shields.io/badge/%E6%8D%90%E8%B5%A0-%E6%94%AF%E4%BB%98%E5%AE%9D-blue)](https://res.cloudinary.com/mighil/image/upload/v1578647638/donate-to-mighil.png) [![捐赠](https://img.shields.io/badge/%E6%8D%90%E8%B5%A0-%E5%BE%AE%E4%BF%A1-green)](https://res.cloudinary.com/mighil/image/upload/v1578647638/donate-to-mighil.png)

**Note: You're nothing but an a-hole if you sell EFI folder (config) that's readily available for free.**

# X230 Hackintosh Catalina 10.15.2 Clover & Config.

Fork or star, it's your call.

![X230 from 2012 Living The Catalina Dream!](https://i.redd.it/2vvckrfosi941.jpg)

EFI Folder (Clover), plist, and BOOT required to install/run Thinkpad X230 Hackintosh Catalina 10.15.2 & 10.15. Move these files to your EFI Folder. I've got another EFI folder labelled **10.15-test/EFI**. Feel free to tinker that also. 

## #README

- Proceed with caution.
- N/A for Opencore bootloader. Go ahead though, if you know what you're doing. 
- EFI-swap recommended. I haven't tested these settings against the latest version of Clover.

I added [Realtek WLAN kexts](https://github.com/chris1111/Wireless-USB-Adapter-Clover) to use with the Comfast USB Wi-Fi adapter. You should edit the config. according to your preferences. 

The EFI folder is applicable for Vanilla approach and SSD hot-swap (just replace/paste EFI folder - not recommended though.) 

## WiFi

Inbuit WiFi by-default won't work.

Atheros AR5B95, Lenovo part number 20002357 is a macOS supported/Lenovo-whitelisted card available for X230. You should add IO80211Family.kext to Kexts/Other after installing the card.

Alternativly, you can flash the BIOS and remove the whitelist if you plan to use Broadcom WLAN cards.

Stick with a nano-USB WiFi adapter (something cheap based on Realtek) if you don't want to alter your hardware.

## What Else Doesn’t Work? 

Fingerprint reader & card-reader.

## FAQs. 

- [Reddit Link #1](https://www.reddit.com/r/hackintosh/comments/dfdf3l/x230_from_2012_living_the_catalina_dream/).
- [Reddit Link #2](https://www.reddit.com/r/thinkpad/comments/elqbd5/mighty_x230_still_got_game_catalina_10152/).
- [Reddit Link #3](https://www.reddit.com/r/hackintosh/comments/elqd6k/almost_perfect_thinkpad_x230_running_catalina/).
- I've used [neofetch](https://github.com/dylanaraps/neofetch) to display system specs via Terminal.

# A better screenshot (10.15)

![https://i.redd.it/6rq528gjtgr31.png](https://i.redd.it/6rq528gjtgr31.png)

## How to create a bootable macOS Catalina USB install drive? (on MacOS)

[Refer to this guide from 9to5mac](https://9to5mac.com/2019/06/27/how-to-create-a-bootable-macos-catalina-10-15-usb-install-drive-video/)

## How to create a bootable macOS Catalina USB install drive? (on Windows)

1. Install [Transmac](https://www.acutesystems.com/scrtm.htm) on a Windows machine. It has a 15-day trial period and works flawlessly flashing DMG files to USB.

2. Download the [macOS 10.15.2 with clover dmg file from here](https://mirrors.dtops.cc/iso/MacOS/daliansky_macos/) or other sources you come across Google SERP.

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

### Support
![Donate](https://res.cloudinary.com/mighil/image/upload/v1578647638/donate-to-mighil.png)
