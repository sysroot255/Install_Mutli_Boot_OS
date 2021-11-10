# Let's install Debian 10 buster (server)

**We will proceed in the same way with virtualbox, remove the windows iso file and then attach the debian one.**

![virt1](img/Deb/ArcoLinux_2021-06-27_12-45-12.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-45-37.png)

**Here you have to be careful, for the moment there is only the default bios bootloader (windows bootmanager) so windows will want to start first.**

- Start your virtual machine with debian while pressing several times on the **"ESC"** key on the keyboard.

- Select the option **"BootManager"**, then choose the option **"UEFI VBOX CD-ROM"**.
![virt1](img/Deb/ArcoLinux_2021-06-27_12-46-28.png)
![virt1](img/Deb/ArcoLinux_2021-06-27_12-46-51.png)

**You should arrive at the debian 10 installation screen.**

![virt1](img/Deb/ArcoLinux_2021-06-27_12-47-17.png)

**We select the advanced options and the expert install.**

![virt1](img/Deb/ArcoLinux_2021-06-27_12-47-33.png)

**The installation starts in "expert" mode, we will configure all the steps to install a SERVER version of debian 10 (buster).**

![virt1](img/Deb/ArcoLinux_2021-06-27_12-48-01.png)


- choose language (US for the system language).

![virt1](img/Deb/ArcoLinux_2021-06-27_12-48-24.png)

- Select your country (here Belgium).

![virt1](img/Deb/ArcoLinux_2021-06-27_12-49-02.png)


- Choose the locale for the system US (en_US.UTF8).
- select en_US using the **"SPACE"** key and continue.
> Use the "TAB" key to move through the button choices (useful in TUI mode).

![virt1](img/Deb/ArcoLinux_2021-06-27_12-49-16.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-50-09.png)

- Select the good one ("en_US.UTF8" locale).

![virt1](img/Deb/ArcoLinux_2021-06-27_12-50-21.png)

- Configure the keyboard (Belgian).

![virt1](img/Deb/ArcoLinux_2021-06-27_12-50-40.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-50-57.png)

- Detect and mount CD-rom, on the "usb storage" screen, continue, then the message "cd-rom detected" appears, continue.

![virt1](img/Deb/ArcoLinux_2021-06-27_12-51-11.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-51-27.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-51-43.png)

- Load installer components from CD.

>In this step you will be offered to load additional firmwares in the event that it would be useful to you, here we do not need it, just using the **"TAB"** key to go to **"continue"** .

![virt1](img/Deb/ArcoLinux_2021-06-27_12-51-54.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-52-10.png)

- Loading components........

![virt1](img/Deb/ArcoLinux_2021-06-27_12-52-25.png)

- Detecting Network and hardware, configure Network

    1. Say "yes" to auto-configure network.
    2. Waiting time leave to "3" by default.
    3. Set an hostname for your machine and continue.


![virt1](img/Deb/ArcoLinux_2021-06-27_12-52-45.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-53-06.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-53-19.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-53-33.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-53-57.png)

- Set up users and password.

![virt1](img/Deb/ArcoLinux_2021-06-27_12-54-16.png)

    1. Say "yes" to enable shadow password.

![virt1](img/Deb/ArcoLinux_2021-06-27_12-54-34.png)


    2. Say "No" to allow login as root" (only use sudo).

![virt1](img/Deb/ArcoLinux_2021-06-27_12-54-50.png)

    3. Define a user name and password.

![virt1](img/Deb/ArcoLinux_2021-06-27_12-55-05.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-55-25.png)

- Configure The clock.


![virt1](img/Deb/ArcoLinux_2021-06-27_12-55-43.png)

    1. Say "yes" for using NTP.

![virt1](img/Deb/ArcoLinux_2021-06-27_12-56-01.png)

    2. Leave default address server and continue.

![virt1](img/Deb/ArcoLinux_2021-06-27_12-56-15.png)
    
    3. Select time zone (Europe/Brussels)

![virt1](img/Deb/ArcoLinux_2021-06-27_12-56-28.png)


- Partition Disks **(IMPORTANT SECTION)**.

![virt1](img/Deb/ArcoLinux_2021-06-27_12-56-59.png)

    1. Select ""Manual method"".

![virt1](img/Deb/ArcoLinux_2021-06-27_12-57-39.png)

    2. On the next screen we can see our first (#) 3 partitions already used for EFI and windows, so we will go to the "FREE SPACE" part to create a "SWAP" partition first.


![virt1](img/Deb/ArcoLinux_2021-06-27_12-58-10.png)

    3. Press "enter" and create a new partition.

![virt1](img/Deb/ArcoLinux_2021-06-27_12-58-23.png)

    4. Choose a size (for example 4 GB) and continue.

![virt1](img/Deb/ArcoLinux_2021-06-27_12-58-50.png)

    5. Leave location at "beginning" and continue.

![virt1](img/Deb/ArcoLinux_2021-06-27_12-59-05.png)

    6. On "how to use this partition" select "swap area" and continue.

![virt1](img/Deb/ArcoLinux_2021-06-27_12-59-35.png)

    7. on the nex screen, select "Done settings and up the partition".

![virt1](img/Deb/ArcoLinux_2021-06-27_12-59-56.png)

    8. Now we must create an "ext4" partition for de system (where the installation must be done for debian)

![virt1](img/Deb/ArcoLinux_2021-06-27_13-00-17.png)

    9. Go to "FREE SPACE" and create one , It's the same procedure as for the swap but you just have to be careful when choosing the partition type.

![virt1](img/Deb/ArcoLinux_2021-06-27_13-00-34.png)

    10. Choose a size for your server partition (10GB) and continue.

![virt1](img/Deb/ArcoLinux_2021-06-27_13-00-53.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_13-01-12.png)

    11. Choose as type : "ext4 journaling file system".

![virt1](img/Deb/ArcoLinux_2021-06-27_13-01-44.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_13-01-59.png)

    11. There you have it, the ext4 partition is created, you still have to choose "finish partitioning and write changes to disk", say "yes" to write.

![virt1](img/Deb/ArcoLinux_2021-06-27_13-02-41.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_13-03-05.png)

- Install the base system.

![virt1](img/Deb/ArcoLinux_2021-06-27_13-03-25.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_13-03-39.png)

    1. On "Kernel to install" choose "linux-image-amd64".

![virt1](img/Deb/ArcoLinux_2021-06-27_13-05-19.png)

    2. On "drivers to include" select default "generic with all available drivers".

![virt1](img/Deb/ArcoLinux_2021-06-27_13-05-58.png)

- Configure the package manager.

![virt1](img/Deb/ArcoLinux_2021-06-27_13-07-16.png)

    1. Say "no" to "scan an other cd or dvd"

![virt1](img/Deb/ArcoLinux_2021-06-27_13-07-34.png)

    2. Say "yes" on "use a network mirror", choose Belgium and select any mirror archive server and continue.

![virt1](img/Deb/ArcoLinux_2021-06-27_13-07-47.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_13-08-08.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_13-08-24.png)

    3. For "Http proxy" leave blank and continue, for using contrib say "no" .

![virt1](img/Deb/ArcoLinux_2021-06-27_13-08-36.png)

![virt1](img/Deb/ArcoLinux_2021-06-27_13-08-55.png)

    4. For "enabling repository in APT" say "yes".

![virt1](img/Deb/ArcoLinux_2021-06-27_13-09-11.png)

    5. On "service to use" leave default and continue.

![virt1](img/Deb/ArcoLinux_2021-06-27_13-09-43.png)

- Select and install software.

![virt1](img/Deb/ArcoLinux_2021-06-27_13-10-10.png)

    1. For "Update management system" say "yes" or "no" whether security updates can affect the entire system.

![virt1](img/Deb/ArcoLinux_2021-06-27_13-14-41.png)

    2. For "choose software to install" select only component for a server (desktop environnement not installed) and continue.

![virt1](img/Deb/ArcoLinux_2021-06-27_13-15-29.png)

**For the next step: it is important to know if you need "GRUB" yes or not, if your multi boot consists only of "windows" and "debian" then you can install grub on the disk "/ dev / sda "we will not see these steps for this installation because we will be installing archlinux as well and grub at the same time.**

    1. Here we skip the grub installation step by choosing "continue without grub".


![virt1](img/Deb/ArcoLinux_2021-06-27_13-17-23.png)

    2. choose continue at this step :

![virt1](img/Deb/ArcoLinux_2021-06-27_13-17-37.png)

    3. Now finish the installation

![virt1](img/Deb/ArcoLinux_2021-06-27_13-19-38.png)


>Your virtual machine will restart but still without GRUB and will still try to launch windows automatically, this is why it is important to shutdown your virtual machine in order to be able to follow the next step: archlinux install

---

[Let's move on to installing Archlinux with GRUB](https://github.com/sysroot255/Install_Mutli_Boot_OS/blob/master/step5_install_Archlinux_with_grub_and_desktop_environnement.md)
