## How to install Ubuntu 18.04 LTS alongside with Win10

### 1. Make a backup [Optional]

**It's always wise to make a backup.** Backup your important files in advance in case something unexpected occurs.



### 2. Downloading Ubuntu image

For this part, you could go to [How to install Ubuntu 18.04 LTS on VirtualBox](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_virtualbox.md).



### 3. Prepare a bootable USB

- **In Win10 OS, press win+R and type `msinfo32.exe`** This step is to check if your Win10 is booted in UEFI or Legacy BIOS mode. In the right pane of **System Summary**, you can see the **BIOS Mode** line. 

  ![legacy bios mode](images/8cb6bd7b34f9f97524c9e6f47a3997db10eb313967b1ec16152e7c2626d8825e.png)

  ![uefi bios mode](images/5049d79d058ff3da5b685f5b7b2156a6fc163be286721e0faf779eb1630a9821.png)

- **Install Rufus USB creater** You can download Rufus from [here](https://rufus.akeo.ie/).

- **If it's UEFI, plugin your USB disk and apply the following settings**

  ![create ubuntu bootable usb](images/39e5573ba933dcce099238468fda65fbc223f8aa7ce1dbc0cbf792af3e640a49.png)



### 4. Partition the disk on Win10 [Optional]

- **If you install Ubuntu on another hard drive, you may skip this step.**

- **Open Disk Management of Win10.**

  ![Open Disk Management Windows 10](images/6f8d4d3e39acf87a7374aa9d7afa6d4af6dd898d9e05d7b2beea39579fe0048b.jpeg)

- **Shrink the volume to desired size** Select the hard drive partition you want to shrink. The size depends on the free space on your hard drive. At least 10 GB and 20 GB is recommended. 

  ![img](images/46a655d085fd04aba70c8d028b68c73aacd8343fb4dbb0310b46d92223c94ae4.png)
  
  ![img](images/4d0757840adbad1dcd501d94b097a1ab8b90e499fb9430e716a75c082645ad98.png)
  
  ![img](images/cafaf96827483a44fadfe0f7240f9db9f250eab2ffcde4a2e5bdd8819093abaf.png)



### 5. Reboot the computer and boot from USB

- **You may try `F12`, `F10`, `F8` to enter**. On Dell, Acer, Lenovo or Toshiba laptops, it's the `F12` in most cases. Sometimes `Fn` is required (e.g. `Fn` + `F12`) In **Boot Option Menu**, Move the priority of your USB to the first. The interface varies a little from laptop to laptop.

  ![img](images/c6605e7f44cc7f49e7ad6985beb2fa9ca714aaaa465309b6299432d3343379bb.jpg)

- **Turn off Secure Boot.** Find the **Secure Boot** setting, and if possible, set it to **Disabled**. This option is usually in either the **Security** tab, the **Boot** tab, or the **Authentication** tab.

- **Save and reboot**



### 6. Install Ubuntu

- **Select `Install Ubuntu`** The procedure is similar to that of [How to install Ubuntu 18.04 LTS on VirtualBox](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_virtualbox.md). 

- **You may skip and continue as well.**

  ![dual boot ubuntu and windows 10](images/cf70b8ddcd0fcd0ce99099467bf949e9ded4df1da36e5d8b9831798a92a0e608.png)

- If you want to keep your Windows system, select **Something else** as **Installation type**.

  ![img](images/fffed54f2573b0a6ee807249c3e9d4c81d9bbe1f381cbf63a70ce29413b916b3.png)

- **Choose the partition you just created.**
  
  ![dual boot ubuntu windows 10](images/a4874fc04afc1f72c396472bb15426c435f5185f3f6d1b6fc10fa0df9706748f.png)

- **Create root `/`, swap and home `/home`.** Select **free space**. Click `+`. You could reference the following settings. The `swap area` is recommended to be larger than 6 GB. The `/home` is where you put your personal files, thus make sure it's large enough. Make sure that everything is correct before you click `Install Now`.


  ![Install_Ubuntu_Windows_Dual_Boot_5](images/5a256692862bc5995fbe9624f3c9e26cbd2293b50b8f5f4fc8505dcaa0529dc8.jpeg)

  ![dual boot Windows with Linux](images/ccf9c7026315f015fd663b361e1c0b78bc518d65bcf11a1a5fa77244cbaf3e12.jpeg)

  ![Install_Ubuntu_Windows_Dual_Boot_7](images/0535753e7bf48e3e381113141688782884e94ed840bcca22f995ef86d9e656d9.jpeg)

  ![Install_Ubuntu_Windows_Dual_Boot_8](images/c593dbd913e3d898910d85b6a7ef8ef45f1f99b9518fb039909f9bb785a0701a.jpeg)

  ![installing Ubuntu in dual boot with Windows](images/9652e3692277372a7a82f123558fb70a2a4400055b5bf67c633c479bb9d3fc72.jpeg)




### 7. Reboot and select `Ubuntu`

![dual boot windows and ubuntu](images/2e70c1548fc07139b11ad0f0c4dfd6ab5fbe82fc1aa8fb2829ec89cec96c3dce.jpg)



#### Reference

1. <https://www.easyuefi.com/resource/check-windows-is-booted-in-uefi-mode.html>
2. <https://tutorials.ubuntu.com/tutorial/tutorial-create-a-usb-stick-on-windows#3>
3. <https://www.pcsuggest.com/dual-boot-windows-10-and-ubuntu-uefi/>
4. <https://www.disk-partition.com/windows-10/windows-10-disk-management-0528.html>
5. <https://itsfoss.com/install-ubuntu-dual-boot-mode-windows/>
6. https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/disabling-secure-boot