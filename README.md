# reminders

## Here's a (growing) collection of (mostly linux-related) stuff that I use daily but can't seem to remember.

##### Find usb device name:

```bash
fdisk -l
```

or:

```bash
lsblk
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
 
##### See what process is using port 8081
```bash
lsof -P -i :8081 | grep LISTEN
```

##### Fancy console
```bash
export PS1="🍔  \[\033[01;35m\]\u@\h:\[\033[01;34m\]\[\033[01;32m\]\w \[\033[01;34m\]\n>\[\e[0m\]"
```



