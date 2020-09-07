# tutorials
This repository contains the fundamental tutorials for VE280.

## Linux Setup Tutorials
OS| Title        | Author           | Date  
:-:| :-----------: |:-------------:| :---: 
**Win10 <br>(REC.)**| [ How to install <br>Windows Subsystem <br>for Linux (WSL) <br>on Win10](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_wsl.md) | [Changyuan Qiu](https://github.com/PeterQiu0516) <br>& <br>[Yihao Liu](https://github.com/tc-imba) | 2020-09-07 
Win10| [How to install <br>Ubuntu 18.04 LTS <br>alongside with Win10](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_dual_boot.md) | [Tianyi Ge](https://github.com/TimothyGe) | 2019-05-21 
Win10 <br> & <br> Mac OS| [How to install Linux <br>on Docker](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_docker.md) | [Yihao Liu](https://github.com/tc-imba) | 2019-05-22 
Win10 <br>& <br>Mac OS| [How to install <br>Ubuntu 18.04 LTS <br> on VirtualBox](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_virtualbox.md) | [Tianyi Ge](https://github.com/TimothyGe) | 2019-05-15 
Win10 <br>& <br>Mac OS| [How to install <br>Ubuntu 18.04 LTS <br>on VMware Fusion](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_vmware.md) | [Jiayi Chen](https://github.com/Janecjy)<br> &<br>[Zian Ke](https://github.com/zianke) | 2019-05-15 

**Further Notes**:

To speed up your downloading, you may change your source list to SJTU source by typing the command below.

```
sudo sed -i 's/archive.ubuntu.com/ftp.sjtu.edu.cn/g' /etc/apt/sources.list
```

Then update the list of available packages before installing any of them.

```
sudo apt update
```

Now you can install packages from the SJTU source, for example, `build-essential`, which includes `gcc`, `g++`, `make`, etc.

```
sudo apt install build-essential
```


## Other Fundamental Tutorials 
| Title        | Author           | Date  |
| ------------- |:-------------:| ----- |
| [An elementary introduction to GitHub](https://github.com/ve280/tutorials/blob/master/github_introduction.md) | [Zian Ke](https://github.com/zianke) | 2019-05-27 |
| [Submit your VE280 project solution to Joint Online Judge (JOJ)](https://github.com/ve280/tutorials/blob/master/joj_project_submission.md) | [Zian Ke](https://github.com/zianke) | 2019-05-20 |



