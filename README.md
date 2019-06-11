# alarm-chroot

ArchLinuxARM chroot script for Raspberry Pi 2/3

Reference 
---------

1. https://disconnected.systems/blog/raspberry-pi-archlinuxarm-setup/
2. https://web.archive.org/web/20170710194700/https://wiki.archlinux.org/index.php/Raspberry_Pi#QEMU_chroot

Requirements
------------

An ArchLinux x86_64 machine and core utilities.

```sh
pacman -S qemu wget arch-install-scripts parted
yay -S qemu-user-static
systemctl start systemd-binfmt
```

HOWTO:

1. Edit `activate` script and set `SETUP=true` if running for the first time
2. Run `sudo ./activate`
