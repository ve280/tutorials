## How to install Ubuntu 18.04/20.04 LTS on VMware Workstation/Fusion

### 1. Download Ubuntu image

- **Open the Ubuntu website.** Go to the official website <https://www.ubuntu.com/download/desktop>. You can download the Ubuntu disk image (also known as an ISO file) here. For VE280 SU2020, both **Ubuntu 20.04 LTS** and **Ubuntu 18.04.2 LTS** are recommended. We'll take the latest version as an example. You can find older releases on <https://releases.ubuntu.com>.

  ![ubuntu.png](images/5tYugfmb68.png)

### 2. Download VMware Workstation/Fusion

- **For SJTUers.** SJTU provides free version of VMware at this link: <http://vmap.sjtu.edu.cn>. Login with jAccount, then you can see all the available products. For Mac users, please choose **VMware Fusion 11.x Pro (for Intel-based Macs)**. For Windows users, please choose **VMware Workstation 15.x Pro**. We'll use VMware Fusion in this tutorial. But the steps of VMware Workstation should be similar.

  ![products](images/2020-05-12_160400.png)

- **Click "Add to Cart".**

  ![addtocart1](images/msedge_87ehVOVhyj.png)

  ![addtocart2](images/msedge_ZMHxBB4Fk9.png)

- **Click "Check Out".**

  ![checkout](images/Snipaste_2020-05-12_16-17-13.png)

- **Fill in the "Contact Information" section.** Then click "Proceed with Order". You'll be shown with the order details.

  ![contact](images/msedge_glKeThc0f0.png)

- **Keep your Serial Number.** Copy your Serial Number to somewhere in order to make it persistent. You'll need this to activate VMware Fusion on your Mac. Then click "Download".

  ![serial](images/f205db997db3a42b44e0e04538edc88342d6e3a1801d9f5d5e769dfaa71bd9df.png)

- **For free trial.** If you don't have a valid SJTU account, you can download a 30-day free-trial version on <https://www.vmware.com>. Login the website. If you don't have an account, sign up first.

  ![download1](images/msedge_ffPjy92rEo.png)

  ![download2](images/msedge_fIJsZuNebj.png)

  ![download3](images/msedge_cgJUYfQGkW.png)
  
  ![download4](images/msedge_Xrj1LbuxjN.png)
  
  ![download5](images/msedge_ZH5R6QXrss.png)
  
  ![download5](images/msedge_1WnQbR0xEi.png)
### 3. Install VMware Workstation/Fusion.

#### 4.1 For VMware Fusion

After the download is finished, you can install VMware Fusion on your Mac. Please paste your Serial Number here and click "Continue". 

  ![serial](images/0404054f7e846808f5b503364bc8d63d02f7562cfd6355a5d3539a5d236eadf8.png)

#### 4.2 For VMware Workstation

- **Run VMware-workstation-full-15.5.2-15785246.exe.**

  ![install1](images/Snipaste_2020-05-12_18-10-18.png)

  ![install2](images/Snipaste_2020-05-12_18-28-07.png)

  ![install3](images/Snipaste_2020-05-12_18-30-36.png)

  ![install4](images/Snipaste_2020-05-12_18-33-14.png)

  ![install5](images/Snipaste_2020-05-12_18-34-45.png)

  ![install6](images/Snipaste_2020-05-12_18-35-55.png)
  
  ![install7](images/Snipaste_2020-05-12_18-41-30.png)
  
  ![install8](images/Snipaste_2020-05-12_18-44-00.png)

- **Run VMware Workstation Pro and input the license key.**

  ![install9](images/Snipaste_2020-05-12_20-29-27.png)

  ![install10](images/Snipaste_2020-05-12_20-31-43.png)

### 4. Install Ubuntu in VMware Workstation/Fusion

#### 4.1 For VMware Fusion

- **Click "+".** On the top-left of the main screen there’ll be a “+” button. Click on it and choose “New…” to create a new VM.

  ![new.png](images/41465e3e8fffb25069dfb40e512c43f629554b8ce138412f9d0160324e9422ec.png)

- **Drag the ISO file icon onto the drop target.** The new virtual machine window will pop up, ready to go. Simply drag the ISO file icon onto the target marked by the red circle.

  ![install.png](images/becf7dc8a799ba113eda87ce943bf596b2b5ea72287726fa7c643487a241efba.png)

- **Click "Continue".** Once the file image is loaded, VMware Fusion for Mac will automatically move to the next step.  VMware Fusion is smart enough to go through the entire Linux setup process without bothering you at all, so this is where you specify your basic account and password. If you want to be able to access your main Mac desktop while within Ubuntu, check “Make your home folder accessible to the virtual machine” too. Then click “Continue”.

  ![linux easy install vmware fusion](images/3be88813b14a481e3c9477ed6a6ac9f6c66320a267eeff10e0a43eaee2bc7d01.png)

- **Click "Finish".** VMware Fusion for Mac completes all the work for you.

#### 4.2 For VMware Workstation

- **Click "Create a New Virtual Machine".**

![create_a_new](images/vmware_xVMXvyLkiL.png)

- **Click "Next >"**

![wizard1](images/vmware_NYFA4OJWTu.png)

- **Choose installer disc image file and Click "Next >"**

![wizard2](images/vmware_e0gX1qnZba.png)

- **Personalize Linux**

![wizard3](images/vmware_Motc5ZNmJ3.png)

- **Name the Virtual Machine**

![wizard4](images/vmware_FjCp4JYqOa.png)

- **Specify Disk Capacity**

![wizard5](images/vmware_AO2HVxAwpC.png)

- **Ready to Create Virtual Machine**

![wizard6](images/vmware_94WEBCSDnw.png)

### 5. Enjoy your journey on Linux

You’ll be prompted to log into your new Ubuntu virtual machine. 

**Ubuntu 18.04 LTS**

![img1](images/30210583be3453983e46fb1e868f4da143b6e3711ec6f91279b5d663158aafaa.jpg)

**Ubuntu 20.04 LTS**

![img2](images/nWmu9VWONM.png)

#### Reference

1. <https://www.askdavetaylor.com/install-ubuntu-linux-vmware-fusion-mac>
2. <http://www.macinstruct.com/node/394>