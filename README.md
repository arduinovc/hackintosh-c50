# Hackintosh-c50

EFI boot folder based on OpenCore for Dynabook Satellite Pro C50-H-101  
Last update: May 17th 2024. 

/!\ WARNING = Project in standby. No futur update planned.  

## Description

EFI files based on OpenCore  
OpenCore version: 0.9.9  
Seems to be compatible with: macOS Sonoma    
Test status: installed.  

## How to use  

1/ Download a release corresponding to your macOS version  
2/ Extract it on USB stick (GPT disk with FAT32 primary partition) or EFI partition  
3/ Generate a new "SystemSerialNumber" and "SystemUUID" using OCAuxiliaryTools for example  
4/ Save and reboot  

## Hardware

__Laptop Dynabook Satellite Pro C50__  
![Dynabook C50-H-101](/Assets/Dynabook-C50.JPG "Dynabook C50")  
[Datasheet Toshiba](/Assets/Dynabook-C50-H-101-Datasheet-DE.pdf)  


| Type	| Name                   |
|:------|:-----------------------|
| CPU	| Intel i5 gen 1035G1	 |
| RAM	| 8Gb DDR4 3200 MHz  |
| GPU	| Intel UHD G1 |
| Drive	| NVMe SSD 256 Gb	 |
| Sound	card	| Realtek ALC256	 |
| WLAN	| Intel Wireless 3165 	 |
| Bluetooth | Intel Wireless 3165 #Port0?? |
| LAN	| Realtek RT8111 |
| Display | LVDS or eDP display 1920*1080 |

## SMBIOS Info

System Product Name : MacBookAir9,1  
System Serial : FVFD66Z9MNHP  

## Working and Not-Working

### Working (at this point)  
MacOS Sonoma installed successfully.  
Support native 1080p screen and backlight is on.  
Support Intel Wireless network card and Ethernet Realtek card.  
SSD (Sata) is detected correctly.  
Bluetooth works (enable and connect devices - Apple Magic Mouse 2 works).  
Video acceleration fixed with device-id spoofing.  

### Not-Working  
Touchpad/Trackpad: VoodooPs2/VoodooI2C don't work.  
Keyboard Fn function doesn't work at the moment.  
Find my : wrong position or no position reported at all.

## Screenshots

![Dynabook C50-H-101](/Assets/Sonoma.png "C50 Sonoma")
![Dynabook C50-H-101](/Assets/Sonoma-SystemInfo.png "C50 Info")
![Dynabook C50-H-101](/Assets/Sonoma-SystemSettings.png "C50 System Settings")
![Dynabook C50-H-101](/Assets/Sonoma-MapsStore.png "C50 Maps and Apple Store")

## Work to do

Fixing keyboard Fn function and touchpad.  
Fixing screen backlight.  
Control CPU power/frequency change.  

## Credit

Just myself. EFI build from scratch.  
Thx Dortania for OpenCore guide.  
