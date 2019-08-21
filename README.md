### Archlinux aarch64 for Raspberry Pi

kernel base on [raspberrypi/linux](https://www.github.com/raspberrypi/linux) and rootfs base on [archlinuxarm aarch64](https://archlinuxarm.org/platforms/armv8/generic)
Suitable for Raspberry pi 3B, 3B+, 3A, 4B

### Getting Started
Download the [archlinux-aarch64-rpi.img](https://www.hsxsix.com/archlinux-aarch64-rpi.img) or [archlinux-aarch64-rpi.tar.gz](https://www.hsxsix.com/archlinux-aarch64-rpi.tar.gz),
and install images, if you don't know how to install, please read raspberry official installation documentation
at [install images](https://www.raspberrypi.org/documentation/installation/installing-images/README.md).

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

### Notice

#### for aur helper
at /root has a yay package, if you want to install an [aur helper](https://wiki.archlinux.org/index.php/AUR_helpers) tools, [yay](https://github.com/Jguer/yay) is a good choice.
```
pacman -U yay-xxx.xz
```

#### for mirrors
the [archlinux mirrors](https://wiki.archlinux.org/index.php/Mirrors) default is "https://mirrors.tuna.tsinghua.edu.cn/",
please change according to your country and region.

#### GPIO

```
# pacman -S python python-pip
# pip install RPi.GPIO
```
RPi.GPIO works well

### Issue
Personal production, there are many unknown problems.

If you encounter an unresolved problem during use, please submit an issue for me.
