# kali Parallels-Tools-installation
kali 安装及更新镜像源、tools


# 设置镜像源
- sudo（su)
- nano /etc/apt/sources.list
## 这里提供中科大、阿里云、和官方镜像
## ！！！强烈建议使用官方镜像源！！！

### 官方原版

- deb https://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib
- deb-src https://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib

### 中科大
- deb http://mirrors.ustc.edu.cn/kali sana main non-free contrib 
- deb http://mirrors.ustc.edu.cn/kali-security/ sana/updates main contrib non-free 
- deb-src http://mirrors.ustc.edu.cn/kali-security/ sana/updates main contrib non-free
### 阿里云kali源 
- deb http://mirrors.aliyun.com/kali sana main non-free contrib 
- deb http://mirrors.aliyun.com/kali-security/ sana/updates main contrib non-free 
- deb-src http://mirrors.aliyun.com/kali-security/ sana/updates main contrib non-free
### 163网易 Kali源
- deb http://mirrors.163.com/debian wheezy main non-free contrib 
- deb-src http://mirrors.163.com/debian wheezy main non-free contrib 
- deb http://mirrors.163.com/debian wheezy-proposed-updates main non-free contrib 
- deb-src http://mirrors.163.com/debian wheezy-proposed-updates main non-free contrib 
- deb-src http://mirrors.163.com/debian-security wheezy/updates main non-free contrib 
- deb http://mirrors.163.com/debian-security wheezy/updates main non-free contrib

### 阿里云 Kali源
- deb http://mirrors.aliyun.com/kali kali main non-free contrib
- deb-src http://mirrors.aliyun.com/kali kali main non-free contrib
- deb http://mirrors.aliyun.com/kali-security kali/updates main contrib non-free

### 中科大 Kali源
- deb http://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib
- deb-src http://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib

### 浙江大学 Kali源
- deb http://mirrors.zju.edu.cn/kali kali-rolling main contrib non-free
- deb-src http://mirrors.zju.edu.cn/kali kali-rolling main contrib non-free

### 东软大学 Kali源
- deb http://mirrors.neusoft.edu.cn/kali kali-rolling/main non-free contrib
- deb-src http://mirrors.neusoft.edu.cn/kali kali-rolling/main non-free contrib

### 重庆大学 Kali源
- deb http://http.kali.org/kali kali-rolling main non-free contrib
- deb-src http://http.kali.org/kali kali-rolling main non-free contrib

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

# 对了，如果还是显示error，重启吧，基本上没问题了
# 目前parallels 13.3版本支持的tools工具与kali 2018.2版本的内核不兼容安装会出现error could not build kernel modules问题尝试更换低内核版本，另外，如果之前成功安装了parallels tools之后更新到最新版之后会出现黑屏的情况，请选择linux 4.14.0版本可正常运行
