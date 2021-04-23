# This is a small guide for root X96Q Android TV 10.0 and Restore stock firmware with Allwinner H313 SoC
- Device information: X96Q_AndroidTV10.0_sdk29_AllWinnerH313
- Build_number: X96Q_20200504-1405
- Android: 10.0 (sdk29) 
- Chipset: AllWinner H313

## Requirement
- [Download resources file](https://github.com/HungThinh0710/X96Q_AndroidTV_Root_and_Restore_Firmware_Method/releases)
- Installed adb drivers
- A to A Cable (Of course)
- A computer (I'm using Windows 10 64bit)
- A stock firmware (If you want restore your Android TV)

## Method to root
- Install latest Magisk Manager (now is 22.1)
- Copy file `magisk_patched-22100_XSRyq.img` to your usb
- Plug your USB at port 2 (near CARD)
- Plug A-to-A cable to your computer
- Open Command Prompt
- Run command `adb shell` then run `su`
- After that inject patched-boot with command `dd if=/sdcard/magisk_patched-22100_XSRyq.img of=/dev/block/by-name/boot`
- Run `adb reboot` and now, your android TV is rooted with Magisk

# Notes: With Android 10 you can not modify the system partition (It's read-only)

## Method to restore stock firmware
- Install Driver Assisstant
- Open `PhoenixSuite v1.10`, switch to Firmware Tab and select `img` firmware.
- Open `Device Manager`
- Turn off your AndroidTV
- Find a small stick and inject to AV port (It have a hidden button)
- Press and hold that hidden button and plug your cable into USB (port 1). Note (You must hold the hidden button when plug USB cable into android box and pc)
- Now you will see the `Unknown device or something with warning label`in Device manager (At this step, you can free your hand)
- Right click with warning label driver -> select Update Driver 
- Continue choose -> Browse my computer for drivers -> Browse -> Navigate to PhoenixSuite folder and select `Drivers\AW_Driver`.
- Then update the drivers.
- Now you can restore/upgrade/flash your android TV with the firmware
