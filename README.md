# Arch Setup Framework

1.  Boot in Arch Linux ISO
2.  Execute

        pacman -Sy git

3.  git clone this project

        git clone https://github.com/setupfw/arch-sf

4.  edit `./config`, refer to `./samples/config-*`
5.  run `./start`

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
