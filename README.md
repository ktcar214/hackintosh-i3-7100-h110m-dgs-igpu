# hackintosh-i3-7100-h110m-dgs-igpu
Hackintosh configs used for successful installation of macOS Big Sur and Monterey.
+ FileVault works.

## Hardware

* Installation made on 16 December 2021.
* CPU: Intel i3-7100
* Mainboard: ASRock H110M-HDV
  * No HDMI port on the board. Used DVI-HDMI Cable but didn't changed the port setting to DVI (doing so results in pinky display.)
* RAM:16G
* Installed on CZ880(128G) w/ firmware upgrade(latest) in order to make my drive recognized as SSD
  * You're strongly recommended to use SSD. Even making CZ880 recognized as SSD made a significant performance improvement.
* Used latest Opencore, WEG and other kexts up-to-date as of the installation date.
* Followed Opencore Vanila guide.
* BIOS setting: enable iGPU. Others are same as the guide but I enabled VT-d and fixed config.plist accordingly.

## Problem
* No sleep.(Display, System) I wasn't able to figure out why.
* USB 2.0 ports: Two backside USB 2.0 Ports close to speaker connector and all of front usb 2.0 ports won't work.
  * All USB 3.0 ports work well.
  * Location of working and not working usb ports on Motherboard back panel:

---(DVI)----(USB3)---(USB2 under LAN - work) --(USB2 near sound - doesn't work) --- audio
  * I couldn't map those not working ports.
