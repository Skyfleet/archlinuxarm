# Arch Linux ARM image creator
Shell script that creates an Arch Linux image for various SBCs
Tested on Arch Linux

## Prerequisites
- bsdtar
- dosfstools
- parted
- wget
- gnome-disks-utility
- qemu-arm-static

## Building new images from source

Download the script and make it executable:
```
git clone https://github.com/Skyfleet/archlinuxarm
cd archlinuxarm
chmod +x *.sh
```
Note: *any packages included in the bootstrap directory will be installed to the created image*

Run the script as root and select your board from the prompt:
```
sudo ./image-creator.sh -v
```

After this, the image has been created.

*Release images in this repository are configured for DHCP*

At this point, you will want to continue to the [image installation and configuration guide](/IMG_CONFIG.md)
