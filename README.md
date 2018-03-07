# kali Parallels-Tools-installation
kali 安装及更新镜像源、tools


# 设置镜像源
- sudo（su)
- nano /etc/apt/sources.list
## 这里提供中科大、阿里云、和官方镜像
## ！！！强烈建议使用官方镜像源！！！
### 中科大
- deb http://mirrors.ustc.edu.cn/kali sana main non-free contrib 
- deb http://mirrors.ustc.edu.cn/kali-security/ sana/updates main contrib non-free 
- deb-src http://mirrors.ustc.edu.cn/kali-security/ sana/updates main contrib non-free
### 阿里云kali源 
- deb http://mirrors.aliyun.com/kali sana main non-free contrib 
- deb http://mirrors.aliyun.com/kali-security/ sana/updates main contrib non-free 
- deb-src http://mirrors.aliyun.com/kali-security/ sana/updates main contrib non-free

### 官方原版

- deb https://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib
- deb-src https://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib

#### -----无用的镜像源可以用#来注释掉------

## 设置好后依次执行以下命令


- apt-get clean
- apt-get update
- apt-get upgrade -y
- apt-get dist-upgrade -y
- apt-get install dkms kpartx printer-driver-postscript-hp


## 把Parallels-Tools文件考出来

## 命令行中

- chmod -R 777 .
### 设置文件读取权限


## 最后
- ./install

## ok


