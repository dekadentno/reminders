# reminders

Here's a (growing) collection of (mostly linux-related) stuff that I use daily but can't seem to remember.

Find usb device name:

```bash
fdisk -l
```

Bake bootable usb:

```bash
mkfs.vfat /dev/sdXY
umount /dev/sdXY
dd if=PATH_TO_ISO.iso of=/dev/sdX
```

Install missing dependencies:

```bash
apt-get -f install
```

Add existing project to github:

```bash
git init
git add .
git commit -m "First commit"
git remote add origin REMOTE URL
git remote -v
git push origin master
```
