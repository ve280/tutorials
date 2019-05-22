# tutorials
This repository contains the fundamental tutorials for VE280.

| Title        | Author           | Date  |
| ------------- |:-------------:| ----- |
| [How to install Linux on Docker](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_docker.md) | [Yihao Liu](https://github.com/tc-imba) | 2019-05-22 |
| [How to install Ubuntu 18.04 LTS alongside with Win10](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_dual_boot.md) | [Tianyi Ge](https://github.com/TimothyGe) | 2019-05-21 |
| [Submit your VE280 project solution to Joint Online Judge (JOJ)](https://github.com/ve280/tutorials/blob/master/joj_project_submission.md) | [Zian Ke](https://github.com/zianke) | 2019-05-20 |
| [How to install Ubuntu 18.04 LTS on VirtualBox](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_virtualbox.md) | [Tianyi Ge](https://github.com/TimothyGe) | 2019-05-15 |
| [How to install Ubuntu 18.04 LTS on VMware Fusion](https://github.com/ve280/tutorials/blob/master/ubuntu_installation_vmware.md) | [Jiayi Chen](https://github.com/Janecjy), [Zian Ke](https://github.com/zianke) | 2019-05-15 |

**Notes**:

To speed up your downloading, you may change your source list to SJTU source by typing the command below.

```
sudo sed -i 's/archive.ubuntu.com/ftp.sjtu.edu.cn/g' /etc/apt/sources.list
```

Then update the list of available packages before installing any of them.

```
sudo apt update
```

Now you can install packages from the SJTU source, for example, `build-essential`, which include `gcc`, `g++`, `make`, etc.

```
sudo apt install build-essential
```

