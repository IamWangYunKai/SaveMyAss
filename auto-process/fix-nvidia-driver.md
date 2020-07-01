# NVIDIA驱动修复

### 第一：安装ppa的显卡驱动源

```bash
sudo add-apt-repository ppa:graphics-drivers/ppa
sudo apt update
```

### 第二：检查显卡和推荐驱动

```bash
ubuntu-drivers devices
```

现实如下结果：


```bash
name@ubuntu:~$ ubuntu-drivers devices
== /sys/devices/pci0000:00/0000:00:03.1/0000:07:00.0 ==
modalias : pci:v000010DEd00001F06sv00001B4Csd000013A3bc03sc00i00
vendor   : NVIDIA Corporation
driver   : nvidia-driver-440 - distro non-free recommended
driver   : nvidia-driver-435 - distro non-free
driver   : xserver-xorg-video-nouveau - distro free builtin
```

推荐的是440显卡。

### 第三：安装

```bash
sudo apt install nvidia-driver-440
```

### 第四：重启并检查：

```bash
nvidia-smi
```