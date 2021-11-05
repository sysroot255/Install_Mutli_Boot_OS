# Let's install a version of Windows.

**We are going in "virtualbox" to change the ISO file for this time to start on Windows.**

![virt1](img/Win/ArcoLinux_2021-06-27_12-27-41.png)

- For the moment on the storage section on virtualbox, let's delete the archlinux iso file to attach the one for the chosen windows version
![virt1](img/Win/ArcoLinux_2021-06-27_12-28-26.png)
![virt1](img/Win/ArcoLinux_2021-06-27_12-28-52.png)

**Start your virtual machine, you should start installing windows.**

![virt1](img/Win/ArcoLinux_2021-06-27_12-29-28.png)

**Select the installation mode customize in the choice of installation.**

![virt1](img/Win/ArcoLinux_2021-06-27_12-30-38.png)

**We can choose in the unallocated space a size in MB for our windows partition (ex: 40000).**

![virt1](img/Win/ArcoLinux_2021-06-27_12-31-23.png)

**Apply and we can see that windows has created two partitions, a reserved partition and an NTFS primary partition for the system.**

![virt1](img/Win/ArcoLinux_2021-06-27_12-31-41.png)

>(note to understand the different partitions under linux and windows)

1. /dev/sda1 sda1 is to the UEFI (ESP) partition created for all of our systems.
2. MSR(reserved) is /dev/sda2
3. Principal (40GB NTFS) is /dev/sda3

**Let's continue the installation.**

![virt1](img/Win/ArcoLinux_2021-06-27_12-31-54.png)

- Follow all the windows installation steps (choose user, password, preferences etc ...)

**In the end windows is well installed and we are done for this part, shut down your virtual machine.**

![virt1](img/Win/ArcoLinux_2021-06-27_12-44-36.png)


---

[Let's move on to installing Debian 10](https://gitea.86thumbs.net/Abdellah/Multiboot_os/src/branch/master/step4_install_Debian_buster_server_with_swap.md)