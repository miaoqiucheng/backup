---
title: shadowsocks代理设置实现访问外网（翻墙）
date: 2016-12-27 12:14:33
tags: 翻墙
comments: true
categories: 技术 
---

# 一 shadowsocks的设置

1. 访问[shadowsocks在Windows下的设置（设置过程参考）](https://github.com/shadowsocks/shadowsocks-windows/wiki/Shadowsocks-Windows-%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E)，其实，最重要的是下面几步
2. 在任务栏找到 *Shadowsocks* 图标
<!-- more -->
3. 在 **服务器** 菜单添加
有个扫描桌面二维码的选项（好像是，要不就自己找找），把下面的二维码保存并打开，放在桌面上，会自动扫描，扫描完成后保存设置即可。
<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111193327692?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>(这个是我自己用VPS搭建的一个shadowsocks代理，每月1T流量，本人也用不完，所以贴上来，供大家使用，但是如果用的人多了，我就会修改密码了，希望理解。)

# 二 chrome浏览器的设置

## chromre代理插件安装

   [我们用到的是SwitchOmega，具体下载配置请点击本链接。](https://switchyomega.com/)
      
   - 点击扩展程序。

   <div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111193937936?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

   - 把SwitchyOmega.crx拖入界面中，点击添加扩展程序。至此，chrome代理插件安装完成。

   <div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111194244633?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

## chrome浏览器详细配置

   - 打开SwitchOmega的选项（即进行SwitchOmega的设置）
        
        *点击最下方的“**选项**”*
		<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111200159311?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

	- 跳过教程

		<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111194456194?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

	- 点击新建情景模式

		<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111194650541?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

	- 设置情景模式名称，名字可以随便取，最好为英文，如ss。

		<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111194825370?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

	- 代理协议选择SOCKS5

		<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111194935355?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

	- 代理服务器为127.0.0.1
	- 代理端口随便选，不要跟自己使用的端口冲突即可。可以选择1080或者1081等。

		<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111195116028?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>
		<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111195143110?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

	- 点击应用选项即可

		<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111195246403?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

	- 浏览器中会出现一个小圆圈，单击选择ss（自己起的情景模式的名字）。

		<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170111195448685?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

     至此可以上谷歌了。
	 手机操作系统可以自行百度设置办法。至于Linux设置，我就不详细陈述了，如有不懂，可以私信我。
