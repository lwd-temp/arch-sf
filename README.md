# Arch Setup Framework

1. Boot in Arch Linux ISO
2. git clone this project
3. edit `./config`, refer to `./samples/config-*`
4. run `./prefix`
5. run `archinstall`, **donot reboot**
6. run `./postfix`

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
