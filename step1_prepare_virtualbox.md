# Let's configure virtualbox .

**Create a new virtualbox (New), set a name like "Multios" or other.(Select for type "Linux" and for version " Archlinux 64 beacause we will start part of the partitioning with archlinux)**
    

![virt1](img/Win/ArcoLinux_2021-06-27_12-02-27.png)

**Choose the memory size (4GB) for example.**

![virt1](img/Win/ArcoLinux_2021-06-27_12-03-32.png)

**Create a new virtual hard disk [VDI](https://www.makeuseof.com/tag/3-websites-to-download-virtual-disk-images-for-virtualbox/)**

![virt1](img/Win/ArcoLinux_2021-06-27_12-03-58.png)
![virt1](img/Win/ArcoLinux_2021-06-27_12-04-11.png)
![virt1](img/Win/ArcoLinux_2021-06-27_12-04-24.png)

**Create sufficient disk space to install our 3 operating systems (for ex : 80GB)**

![virt1](img/Win/ArcoLinux_2021-06-27_12-04-47.png)

**Now let's adjust some settings, in virtualbox go to the "settings" option**
1. Go to "System" and enable "EFI Oses spacial".

![virt1](img/Win/ArcoLinux_2021-06-27_12-05-31.png)

2. On "Processor" select more CPU like "4".

![virt1](img/Win/ArcoLinux_2021-06-27_12-05-56.png)

3. Go to "Display" and on "Video memory" add more memory like 64MB or 128MB.

![virt1](img/Win/ArcoLinux_2021-06-27_12-06-22.png)

4. Go to Network and choose "Bridged adapter" or "NAT".

![virt1](img/Win/ArcoLinux_2021-06-27_12-06-44.png)

5. Go to "Storage" and create a new disk optical, attach you Archlinux iso file.

![virt1](img/Win/ArcoLinux_2021-06-27_12-07-11.png)
![virt1](img/Win/ArcoLinux_2021-06-27_12-07-42.png)


**After that you can make "apply" and start you virtual marchine, you must have the next screen :**

![virt1](img/Win/ArcoLinux_2021-06-27_12-08-21.png)


---

[So let's prepare EFI Partition](https://github.com/sysroot255/Install_Mutli_Boot_OS/blob/master/step2_create_EFI_partition_for_all_systems.md)







