# Hackintosh-c50

EFI boot folder based on OpenCore for Dynabook Satellite Pro C50-H-101  
Last update: April 12th 2024. 

## Description

EFI files based on OpenCore  
OpenCore version: 0.9.9  
Seems to be compatible with: macOS Sonoma    
Tested with: installed.  

## How to use

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
| Sound	card	| Realtek ALC	 |
| WLAN	| Intel Wireless 3165 	 |
| Bluetooth | Intel Wireless 3165 #Port0?? |
| LAN	| Realtek RT8211 ?	 |
| Display | LVDS or eDP display 1920*1080 |

## SMBIOS Info

System Product Name : 
System Serial :   

## Working and Not-Working

### Working (at this point)  
MacOS Sonoma installed successfully.  
Support native 1080p screen and backlight is on.  
Support Intel Wireless network card and Ethernet Realtek card.  
SSD (Sata) is detected correctly.  
Bluetooth works (enable and connect devices).  

### Not-Working  
Touchpad/Trackpad: VoodooPs2/VoodooI2C don't work.  
I will try VoodooSMBus emulation soon.  
Keyboard Fn function doesn't work at the moment.  
Backlight not adjustable.  
No video acceleration.  

## Screenshots

In-progress

## Work to do

Build the first EFI

## Credit

