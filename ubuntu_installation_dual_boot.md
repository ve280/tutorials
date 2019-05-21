## How to install Ubuntu 18.04 LTS alongside with Win10

### 1. Make a backup [Optional]

**It's always wise to make a backup.** Backup your important files in advance in case something unexpected occurs.



### 2. Downloading Ubuntu image

For this part, you could go to [How to install Ubuntu 18.04 LTS on VirtualBox](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_virtualbox.md).



### 3. Prepare a bootable USB

- **In Win10 OS, press win+R and type `msinfo32.exe`** This step is to check if your Win10 is booted in UEFI or Legacy BIOS mode. In the right pane of **System Summary**, you can see the **BIOS Mode** line. ![legacy bios mode](https://www.easyuefi.com/images/resource/msinfo32-legacy-bios-mode.png)

  ![uefi bios mode](https://www.easyuefi.com/images/resource/msinfo32-uefi-bios-mode.png)

- **Install Rufus USB creater** You can download Rufus from [here](https://rufus.akeo.ie/).
- **If it's UEFI, plugin your USB disk and apply the following settings**![create ubuntu bootable usb](https://www.pcsuggest.com/wp-content/uploads/2017/09/rufus_create_bootable_USB.png)



### 4. Partition the disk on Win10 [Optional]

- **If you install Ubuntu on another hard drive, you may skip this step**
- **Open Disk Management of  Win10**![Open Disk Management Windows 10](https://www.disk-partition.com/windows-10/images/windows-10-disk-management/open-disk-management-windows-10.jpg)

- **Shrink the volume to desired size** Select the hard drive partition you want to shrink. The size depends on the free space on your hard drive. At least 10 GB and 20 GB is recommended. ![img](https://www.pcsuggest.com/wp-content/uploads/2017/09/disk_management_1.png)![img](https://www.pcsuggest.com/wp-content/uploads/2017/09/disk_management_2.png)![img](https://www.pcsuggest.com/wp-content/uploads/2017/09/disk_management_3.png)



### 5. Reboot the computer and boot from USB

- **You may try `F12`, `F10`, `F8` to enter**. On Dell, Acer, Lenovo or Toshiba laptops, it's the `F12` in most cases. Sometimes `Fn` is required (e.g. `Fn` + `F12`) In **Boot Option Menu**, Move the priority of your USB to the first. The interface varies a little from laptop to laptop.![img](https://www.pcsuggest.com/wp-content/uploads/2017/09/ubuntu_UEFI_boot_menu.jpg)

- **Save and reboot**



### 6. Install Ubuntu

- **Select `Install Ubuntu`** The procedure is similar to that of [How to install Ubuntu 18.04 LTS on VirtualBox](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_virtualbox.md). 
- **You may skip and continue as well**![dual boot ubuntu and windows 10](https://www.pcsuggest.com/wp-content/uploads/2017/09/install_ubuntu_3.png)
- If you want to keep your Windows system, select **Something else** as **Installation type** .![img](https://www.pcsuggest.com/wp-content/uploads/2017/09/install_ubuntu_4.png)

- **Choose the partition you just created.**  ![dual boot ubuntu windows 10](https://www.pcsuggest.com/wp-content/uploads/2017/09/install_ubuntu_5.png)

- **Create root `/`, swap and home `/home`** Select **free space**. Click `+`. You could reference the following settings. The `swap area` is recommended to be larger than 6 GB. The `/home` is where you put your personal files, thus make sure it's large enough.![Install_Ubuntu_Windows_Dual_Boot_5](https://i1.wp.com/itsfoss.com/wp-content/uploads/2014/03/Install_Ubuntu_Windows_Dual_Boot_5.jpeg?resize=627%2C511&ssl=1)

  ![dual boot Windows with Linux](https://i1.wp.com/itsfoss.com/wp-content/uploads/2014/03/Install_Ubuntu_Windows_Dual_Boot_6.jpeg?resize=625%2C511&ssl=1)

![Install_Ubuntu_Windows_Dual_Boot_7](https://i0.wp.com/itsfoss.com/wp-content/uploads/2014/03/Install_Ubuntu_Windows_Dual_Boot_7.jpeg?resize=625%2C513&ssl=1)

![Install_Ubuntu_Windows_Dual_Boot_8](https://i0.wp.com/itsfoss.com/wp-content/uploads/2014/03/Install_Ubuntu_Windows_Dual_Boot_8.jpeg?resize=627%2C512&ssl=1)

![installing Ubuntu in dual boot with Windows](https://i0.wp.com/itsfoss.com/wp-content/uploads/2014/03/Install_Ubuntu_Windows_Dual_Boot_9.jpeg?resize=628%2C511&ssl=1)

Make sure that everything is correct before you clock `Install Now`.



### 7. Reboot and select `Ubuntu`

![dual boot windows and ubuntu](https://www.pcsuggest.com/wp-content/uploads/2017/09/ubuntu_dual_boot_grub_menu.jpg)



#### Reference

1. https://www.easyuefi.com/resource/check-windows-is-booted-in-uefi-mode.html
2. https://tutorials.ubuntu.com/tutorial/tutorial-create-a-usb-stick-on-windows#3
3. https://www.pcsuggest.com/dual-boot-windows-10-and-ubuntu-uefi/
4. https://www.disk-partition.com/windows-10/windows-10-disk-management-0528.html
5. https://itsfoss.com/install-ubuntu-dual-boot-mode-windows/