---
title: ' XX-Net使用：XX-Net在各平台使用方法介绍（一）'
date: 2017-01-11 15:30:19
tags: 翻墙
comments: true
categories: 技术
---
# 使用方法
1. 由于封锁严重，软件自带IP已经被封杀殆尽。因此需要数分钟到数小时的初始化IP扫描，方能正常运行。
<!-- more -->
2. 虽然系统内置了公共appid, 还是建议部署自己的appid，公共appid限制看视频。需要注意的是，只有当你能访问Google之后，才能部署自己的APPID。（以上问题在部署的时候注意一点）
# 概述


1. [获取XX-Net](https://github.com/XX-net/XX-Net/blob/master/code/default/download.md)
2. 设置和初始化：安装、设置完成后，如果无法翻墙，则需要等待后台程序扫描IP（10分钟到数小时）。
3. [可选][创建和使用自己的appid](https://github.com/XX-net/XX-Net/wiki/how-to-create-my-appids)
4. [设置代理](https://github.com/XX-net/XX-Net/wiki/%E8%AE%BE%E7%BD%AE%E4%BB%A3%E7%90%86)
5. [**强烈建议**]获取和配置可靠的浏览器（[Firefox火狐浏览器](https://github.com/XX-net/XX-Net/wiki/%E4%BD%BF%E7%94%A8Firefox%E6%B5%8F%E8%A7%88%E5%99%A8)，或[Chrome谷歌浏览器](https://github.com/XX-net/XX-Net/wiki/%E4%BD%BF%E7%94%A8Chrome%E6%B5%8F%E8%A7%88%E5%99%A8)），并使用[代理切换插件](https://github.com/XX-net/XX-Net/wiki/%E5%AE%89%E8%A3%85%E5%92%8C%E4%BD%BF%E7%94%A8-SwitchyOmega)。

总体来说，使用XX-Net科学上网，大致需要以上步骤，下面分别介绍各个操作系统平台下的使用方法：

# Windows系统

1. 双击 start.vbs或者start.bat启动。Win7/8/10：将提示请求管理员权限（出于安装CA证书的需要）。请点击同意。
2. 启动完毕后，将弹出浏览器，访问 http://localhost:8085/ （配置页面简介）
3. 右下角将出现托盘图标：点击可弹出上述的XX-Net配置页面, 右键可显示常用功能菜单。
4. 第一次启动, 会提示在桌面建立快捷方式,可根据自己需要选择。
5. 推荐使用Chrome浏览器, 安装SwichySharp, 可在XX-Net目录中的SwitchySharp文件夹下找到插件和配置文件。
6. 也可以选择使用Firefox（火狐）浏览器。需手动导入证书
7. 启动失败，请关闭后双击start.bat再次启动程序，把日志发到bug反馈区

- WinXP，需要破解tcp连接数，推荐使用tcp-z
- Win8，win10 的APP，需要使用：https://loopback.codeplex.com/
- Windows Server 2008，需要安装 Visual C++ 2008 Redistributable - x86

针对两种常用浏览器，分别有详细的新手图文教程：使用Firefox浏览器、使用Chrome浏览器
# Mac系统

1. 双击 start 启动
2. 证书将被自动导入，如果还有提示非安全连接，请手动导入data/gae_proxy/CA.crt证书
**注：**
- 命令行启动方式：./start
- 推荐使用Chrome和SwitchyOmega扩展
- 部分版本可能需要手动升级python。命令为：brew upgrade

# Linux系统

1. 我们把解压后的文件夹放在某个目录，并重命名为XX-Net（这一步并非必要，主要是为了好理解。）

2. 进入脚本所在目录：
   ```
   cd ~/XX-Net/code/default
   ```

3. 启动脚本：
   ```
   sudo ./xx_net.sh(输入密码即可开启)
   ```
	![这里写图片描述](http://img.blog.csdn.net/20170111231414124?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)注：我的XX-Net-3.2.8放在主目录下。
	4. 自动导入证书，需安装 libnss3-tools 包
	```
	sudo apt-get install libnss3-tools
	```

	5. 没有安装PyGtk的，需要先安装gtk： 
	```
	sudo apt-get install python-gtk2
	```
	6. 配置http代理 localhost 8087, 勾选全部协议使用这个代理。
	如Firefox，如果管理页面弹不出，请在地址栏输入127.0.0.1:8085，注意和代理端口的区别：
	![这里写图片描述](http://img.blog.csdn.net/20170111231554654?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
	推荐Chrome + SwitchyOmega
	7. ubuntu 下，可能需要安装
	```
	sudo apt-get install python-openssl
	sudo apt-get install libffi-dev
	sudo apt-get install -y python-gtk2
	sudo apt-get install python-appindicator
	sudo apt-get install libnss3-tools
	```
	8. 后台运行：在终端中运行：
	```
	code/default/xx_net.sh start/stop/restart
	```
	9. 开机自启：在/etc/rc.local中添加一行：
	```
	sudo /home/username/xxnet/code/default/xx_net.sh start
	```

## 关于 ArchLinux

- 可能需要的包: python-pyopenssl python2-pyopenssl libffi pygtk python2-notify nss

## 关于 Fedora

- 添加 [FZUG 源](https://github.com/FZUG/repo/wiki/%E6%B7%BB%E5%8A%A0-FZUG-%E6%BA%90)，安装 xx-net
- 执行 xx-net 或 systemctl --user start xx-net (后台)启动
- 配置浏览器代理插件

## 其他平台

- OpenWrt
	[在OpenWrt里运行XX-Net](https://github.com/XX-net/XX-Net/wiki/%E5%9C%A8OpenWrt%E9%87%8C%E8%BF%90%E8%A1%8CXX-Net)
	[在装有梅林固件的Netgear R6300V2上安装XX Net](https://github.com/XX-net/XX-Net/wiki/%E5%9C%A8%E8%A3%85%E6%9C%89%E6%A2%85%E6%9E%97%E5%9B%BA%E4%BB%B6%E7%9A%84Netgear-R6300V2%E4%B8%8A%E5%AE%89%E8%A3%85XX-Net)
- Android
计划开发中
	[Android技术设计](https://github.com/XX-net/XX-Net/wiki/Android%E6%8A%80%E6%9C%AF%E8%AE%BE%E8%AE%A1)
- 附录
	1. 关于服务端
	服务端兼容 GoAgent 3.1.x/3.2.x的客户端
	虽然系统内置了公共appid, 还是建议[部署自己的appid](https://github.com/XX-net/XX-Net/wiki/how-to-create-my-appids)。
    2. 异常处理
	如果出现异常，请翻阅[故障速查手册](https://github.com/XX-net/XX-Net/wiki/%E6%95%85%E9%9A%9C%E9%80%9F%E6%9F%A5%E6%89%8B%E5%86%8C)，查看常见问题和解决方法。

	无法解决的，参考[异常处理](https://github.com/XX-net/XX-Net/wiki/How-to-get-start-error-log)，将问题反馈到：
	https://github.com/XX-net/XX-Net/issues
https://groups.google.com/forum/#!forum/xx-net

提交issue时请贴出状态页、GAE_proxy日志、部署日志，以便开发者和其他用户更好地帮助你。

本文档并非原创，[参考出处](https://github.com/XX-net/XX-Net/wiki/How-to-use)。
