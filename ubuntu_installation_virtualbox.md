## How to install Ubuntu 18.04 LTS on VirtualBox

### 1. Downloading Ubuntu image

**Open the Ubuntu website.** Go to the official website <https://www.ubuntu.com/download/desktop>. You can download the Ubuntu disk image (also known as an ISO file) here. The recommended version for VE280 SU2019 is **Ubuntu 18.04.2 LTS**.

![ubuntu.png](https://raw.githubusercontent.com/ve280/tutorials/master/images/cca039be3668470bbab84a3b8a1d1b6007650906cc5606b6e2663a7261ad9f8c.png)

### 2. Install VirtualBox

**Download VirtualBox if you haven't yet done so.** Go to https://www.virtualbox.org/. The tutorial to install VirtualBox for both Windows and Mac is here <https://www.wikihow.com/Install-VirtualBox>



### 3. Create a Virtual Machine

- **Click "New".** Click the blue badge in the upper-left corner of the VirtualBox window, which opens a pop-up menu. 

- **Enter a name for your virtual machine.** Type whatever you want to name your virtual machine (e.g., Ubuntu) into the "Name" field.

- **Select Linux as the "Type" value.** Expand the "Type" drop-down menu and select **Linux**.

- **Select Ubuntu as the "Version" value.** Make sure **Ubuntu (64-bit)** is selected in the "Version" drop-down menu. Click **"Next"**.

- **Select an amount of RAM to use.** Drag the slider left or right to decrease or increase the amount of RAM that VirtualBox will have available for your Ubuntu virtual machine.

  - The ideal amount of RAM is automatically selected when you get to this page.
  - Make sure not to increase the RAM into the red region; keep the slider in the green region.

  ![img](https://raw.githubusercontent.com/ve280/tutorials/master/images/762fe374bf3f53529eca374ea0ef957a311ad10b37ac65198c604bdfdce49719.png)



- **Choose the File location and File size**. We will be setting the disk type to VDI and the file size to be 40GB. It depends on the free space on your disk. You may apply the default settings.

  ![img](https://raw.githubusercontent.com/ve280/tutorials/master/images/1d3a51165bf99fc160a0e13951804c69b7ea8b4ac69cbf8f830f4d3b14934529.png)



### 4. Install Ubuntu in VirtualBox

- **Double click the virtual machine "Ubuntu" and select your Ubuntu ISO**.

![img](https://raw.githubusercontent.com/ve280/tutorials/master/images/5748390801f48567a0282498f0472c7ce17dcb1e2e89185da7d79a4790c0d0c6.png)

- **Click "Open", then "Start", then "Install Ubuntu"**.

- **Check both boxes on the "Preparing to install Ubuntu" page then "Continue".** This will ensure that everything Ubuntu needs to run will be installed.
- **Check the "Erase disk and install Ubuntu" box then "Install Now".** This may sound scary, but don't worry—nothing on your computer will be erased.
- **Click Continue when prompted.** This confirms that you understand the virtual machine's virtual drive will be "erased" (there's nothing on it anyway) and begins the Ubuntu installation process.



### 5. Setting up Ubuntu

- **Select a time zone then "Continue".** Click a section that correlates with your position on the map. You may choose **"Shanghai"**. 
- **Enter your username, computer's name and password**.![img](https://raw.githubusercontent.com/ve280/tutorials/master/images/ee65ee3813430c3038eeb6761e3f5fb9408eab3527ed3eeb20a58931d0f36d1b.png)
- **Wait for Ubuntu to finish installing.** This process may take anywhere from a couple of minutes to half an hour depending on the performance of your computer.
- **Restart the virtual machine and log in**. Remember your password.



### 6. Enjoy your journey on Linux

![img](https://raw.githubusercontent.com/ve280/tutorials/master/images/30210583be3453983e46fb1e868f4da143b6e3711ec6f91279b5d663158aafaa.jpg)





#### Reference

1. <https://linuxhint.com/install_ubuntu_18-04_virtualbox>
2. <https://www.wikihow.com/Install-Ubuntu-on-VirtualBox>
3. <https://news-cdn.softpedia.com/images/news2/ubuntu-18-04-lts-bionic-beaver-final-beta-released-available-for-download-now-520571-6.jpg>