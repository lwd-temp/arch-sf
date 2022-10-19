# Arch Setup Framework

## Get Started

1. partition your storage disk, using `diskmgmt.msc` on Windows:
   - EFI system partition
   - `/boot` partition, formatted FAT32 better
   - `/` partition, no formatted
2. git clone this into `/boot` partition
3. edit your config refer to samples

### Copy To EFI partition by Windows

run as administrator:

```
mountvol u: /s
git clone https://github.com/setupfw/arch-sf
```

## Usage

1. Boot in Arch Linux ISO
2. mount boot partition, cd it
3. run `./prefix`
4. run `archinstall`, **donot reboot**
5. run `./postfix`

### archinstall

- **Mirror region**

  e.g. press **/** and type `ina` to find **China**

- **Locale language**

  e.g. search `zh_CN`

- **Drive(s)**
- **Disk Layout**

  1. Select what ...
  2. change partitions filesystems correctly
  3. ensure ESP partition
  4. must mount boot & root partition
  5. encrypt root partition

- **Bootloader**: select **GRUB**

- **Hostname**

- **User account**: your sudo user with password

- **Profile**: recommend **desktop/KDE**

- **Audio**: recommend **pipewire**

- **Kernels**: recommend **linux-lts**, but **linux** only if bug

- **Network configuration**: select **NetworkManager** for GUI

- **Timezone**

  e.g. search `hai` to select **Asia/Shanghai**

## Tips

Low Resolution:

press `e` on grub menu, add `nomodeset video=640x360` to the end of `linux`
