# reminders

## Here's a (growing) collection of (mostly linux-related) stuff that I use daily but can't seem to remember.

##### Find usb device name:

```bash
fdisk -l
```

or:

```bash
df
```

##### Make bootable usb:

```bash
mkfs.vfat -n 'Name' -I /dev/sdXY
umount /dev/sdXY
dd if=PATH_TO_ISO.iso of=/dev/sdX
```

##### Install missing dependencies:

```bash
apt-get -f install
```

##### Add existing project to github:

```bash
git init
git add .
git commit -m "First commit"
git remote add origin REMOTE URL
git remote -v
git push origin master
```

##### Show detailed information on the hardware configuration of the machine 
```bash
lshw
```

##### Show I/O usage information (fishy load average)
```bash
iotop
```
##### List directory as tree structure
```bash
tree myDirectory/
```
##### Search for particular string recursively, but don't look in node_modules and dist folders
```bash
grep -Rin "bla" . --exclude-dir=node_modules/ --exclude-dir=dist/
 ```
