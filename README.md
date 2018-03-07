# kali-Parallels-Tools-installation
kali 安装及更新镜像源、tools

中科大
deb http://mirrors.ustc.edu.cn/kali sana主要非免费贡献 
deb http://mirrors.ustc.edu.cn/kali-security/ sana/updates main contrib non-free 
deb-src http://mirrors.ustc.edu.cn/kali-security/ sana/updates main contrib non-free
 阿里云kali源 
deb http://mirrors.aliyun.com/kali sana main non-free contrib 
deb http://mirrors.aliyun.com/kali-security/ sana/updates main contrib non-free 
deb-src http://mirrors.aliyun.com/kali-security/ sana/updates main contrib non-free


deb https://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib
deb-src https://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib

nano /etc/apt/sources.list

apt-get clean
apt-get update
apt-get upgrade -y
apt-get dist-upgrade -y
apt-get install dkms kpartx printer-driver-postscript-hp


