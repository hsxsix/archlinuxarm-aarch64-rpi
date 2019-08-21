### Archlinux aarch64 for Raspberry Pi

kernel base on [raspberrypi/linux](https://www.github.com/raspberrypi/linux)
Suitable for Raspberry pi 3B, 3B+, 3A, 4B

### Getting Started
Download the [archlinux-aarch64-rpi.img](https://www.hsxsix.com/archlinux-aarch64-rpi.img),
and install images, if you don't know how to install, please read raspberry official installation documentation
at [install images](https://www.raspberrypi.org/documentation/installation/installing-images/README.md)
the Wifi Configuration at '/boot/wpa_supplicant.conf', you can add your wifi information to the format inside. 
If there is nothing wrong with it, raspberry pi will automatically connect to your wifi at boot.
The default root password is root.

the first boot, must input 
```
/usr/bin/init_resize
```
or 
```
init_resize
```
to extended rootfs space to the entrie tf card, it will reboot.
next everything is given to google and archlinux wiki!

### ISSUS
If you encounter an unresolved problem during use, please submit an issue for me.
