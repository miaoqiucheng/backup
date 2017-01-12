---
title: ubuntu安装hp-M1136打印机驱动.md
date: 2017-01-09 14:52:20
---
## 下载驱动

 1. [搜索自己打印机型号对应的驱动](http://support.hp.com/us-en/drivers)；
 2.  [这是搜索我的打印机M1136的型号对应驱动](http://support.hp.com/us-en/drivers/selfservice/HP-LaserJet-M1130-Multifunction-Printer-series/5094778/model/4075451)；
 3. 点击**learn more**下载完成后对应的是*hplip-3.16.11.run*文件。

## 安装驱动

```
cd 下载
chmod +x ./hplip-3.16.11.run
sudo ./hplip-3.16.11.run
```
在这一过程中，会出现好多选项，一路同意下去即可。

## 配置打印机

系统设置**->**打印机**->**添加**->**网络打印机**->**使用SAMBA的Windows打印机**->**点击浏览（可能会需要安装一些东西，默认同意即可）
<div align=center>
![这里写图片描述](http://img.blog.csdn.net/20161202202339060)
**->**然后你会找到你所在的局域网的一些设备，这时找到你的打印机，登录即可
**（点击浏览后确认即可）**
<div align=center>
![这里写图片描述](http://img.blog.csdn.net/20161202201701846)![这里写图片描述](http://img.blog.csdn.net/20161202201734761)![这里写图片描述](http://img.blog.csdn.net/20161202201752230)
**（我的打印机名字是911-PC）**
**->**自动弹出一些需要安装的依赖，默认安装即可**->**安装完成后点击前进后显示如下
<div align=center>
![这里写图片描述](http://img.blog.csdn.net/20161202201806152)
**（选择HP）**
<div align=center>
![这里写图片描述](http://img.blog.csdn.net/20161202201820683)
**（由于列表中没有M1136，所以选择M1120作为替补）**

																		    --END
