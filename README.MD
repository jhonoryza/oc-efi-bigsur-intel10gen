# OpenCore 8.7 EFI Mac Os Big Sur

##  Hardware

| Items       | Model               	|
| ----------- | ------------------- 	|
| Motherboard | AsRock H410M 			|
| CPU         | Intel Core i3-10100 	|
| RAM         | KLEVV 2x16G 2666 MHz 	|
| iGPU 		  | UHD 630 				|
| dGPU 		  | GT710 					|
| Sound Card  | Realtek ALC887      	|
| Ethernet    | (Onboard)           	|

## Notes
- iGPU is configured as headless
- GT710 metal support in BigSur OS

##  Functional
- [x] Sound Card
- [x] Network Card
- [x] sleep/wake up
- [x] USB2.0 / USB 3.0
- [x] DP/HDMI Output
- [x] Graphics Acceleration

##  Official Tutorial
- [https://dortania.github.io/OpenCore-Install-Guide/](https://dortania.github.io/OpenCore-Install-Guide/)

## Tools
- [https://github.com/ic005k/OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools), this tool is for create or configure EFI
- [https://github.com/corpnewt/gibMacOS](https://github.com/corpnewt/gibMacOS), this tool to download macos using cli

## General Instruction
- After making bootable mac installer, open OCAuxiliaryTools then mount efi partition on your usb installer
- Copy from this repo EFI folder to mounted efi partition
- Reboot and boot from your usb installer
- Open disk utility, format hardrive with apfs format
- Make sure date is correct, by opening cmd and run date
- Install Mac Os
- After successfully install, Open OCAuxiliaryTools again to mount efi partition from your installed hardrive
- Copy EFI folder (you can grab from this repo or from your usb installer) to mounted efi partition
- Now you can boot to macos normally without usb installer

