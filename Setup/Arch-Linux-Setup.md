# Pre Installation

## Prepare the Bootable USB

- Acquire the installation image (`*.iso*` file) [here](https://www.archlinux.org/download/)
  > Further information about the image acquisition can be seen [here](https://wiki.archlinux.org/index.php/installation_guide#Acquire_an_installation_image).

- Find out the name of the USB drive using the following command.
  ```bash
  $ sudo fdisk -l
  ```
- If it is mounted, unmount it using the following command, replace `/dev/sdxn` with the drive partition:
  ```bash
  $ sudo umount /dev/sdxn
  ```
- Copy the installation image data to the USB using the following command, replace `/dev/sdx` with the USB drive:
  ```bash
  $ dd bs=4M if=path/to/archlinux.iso of=/dev/sdx status=progress oflag=sync
  ```
  > Further information about the USB preparation can be seen [here](https://wiki.archlinux.org/index.php/USB_flash_installation_medium#Using_basic_command_line_utilities)
- Wait until the process finished.

# Installation

# Post Installation