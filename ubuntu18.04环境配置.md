# ubuntu18.04环境配置

## 桌面美化

### 安装工具：Gnome Tweaks

> 安装完拓展不想重启电脑，那就重启gnome吧
>
> ​	Alt + F2
>
> ​	输入r

​	sudo apt-get update

​	sudo apt-get install gnome-tweak-tool

​	sudo apt-get install gnome-shell-extensions

​	sudo apt-get install gnome-shell-extension-dashtodock



### 主题，图标与shell

> 直接用git上的主题和图标(是我现在在用的)
>
> https://github.com/mzy8329/ubuntu_desktop.git



> 连接网站：
>
> ​	https://www.gnome-look.org/
>
> ​	网站提供了许多主题，图标，字体
>
> 把下好的包放在家目录的**./local/share**中的**themes,fonts,icons(主题，字体，图标)**（如果没有将新建一个）

​	在Tweaks->extension->勾选User themes

​	重启gnome

​	在外观里可以对主题图标字体进行选择

​	Dock可以通过 右键dock的方式修改样式

​	终端可以通过 终端--编辑--首选项的方式修改（稍微改一下透明度就好）



## 软件安装

### 安装ROS

> https://www.ros.org/



### 安装Chrome浏览器

​	sudo wget http://www.linuxidc.com/files/repo/google-chrome.list -P /etc/apt/sources.list.d/

​	wget -q -O - https://dl.google.com/linux/linux_signing_key.pub  | sudo apt-key add -

​	sudo apt update

​	sudo apt install google-chrome-stable



### 安装QQ

> 安装deepin-wine环境

​	git clone https://gitee.com/wszqkzqk/deepin-wine-for-ubuntu.git 		

​	cd deepin-wine-for-ubuntu 

​	sudo sh install.sh



> 下载对应的qq,微信等容器，网址：
>
> https://github.com/wszqkzqk/deepin-wine-ubuntu
>
> 下载后到所在路径下

​	sudo dpkg -i  ##安装包的名称##

​	sudo apt-get install -f

微信，百度云等同理



> 解决qq不能正常最小化的问题

​	sudo apt-get install gnome-shell-extension-top-icons-plus

​	在Tweaks->扩展->勾选Topicons plus



### 安装Typora

​	wget -q0 - https://typora.io/linux/public-key.asc | sudo apt-key add -

​	sudo apt-get-repository 'deb https://typora.io/linux ./'

​	sudo apt-get update

​	sudo apt-get install typora



### 安装WPS

> 去官网获得安装包：https://www.wps.cn/product/wpslinux#
>
> 百度云获得字体：链接：https://pan.baidu.com/s/1R1heuryy7jIpv7h2Z30sOw 密码：p9my

​	sudo dpkr -i 包名

​	把字体放到/usr/share/fonts/wps-office路径下	



### 安装CLion

#### 搭环境

​	sudo apt-get update 

​	sudo apt-get install build-essential 

​	sudo apt-get install cmake 

​	sudo apt-get install bison 

​	sudo apt-get install library* 

​	sudo apt-get install libncurses5-dev 

​	sudo apt-get install g++ 

​	sudo apt-get install kdelibs5-dev 

​	sudo apt-get install make

#### 到官网下安装包

> https://www.jetbrains.com/clion/download/#section=linux
>
> 学生账户：
>
> ​	190320205@stu.hit.edu.cn
>
> ​	20010513mzy8329



## 电脑里当然要有游戏了

### 韦诺之战

```
sudo apt-get install wesnoth
```

回合制策略游戏，好玩



### CUBE2

https://sourceforge.net/projects/sauerbraten/files/sauerbraten/2020_11_29/sauerbraten_2020_12_27_linux.tar.bz2/download

3DFPS,好玩