---
title: XX-Net使用：使用chrome浏览器（二）
date: 2017-01-12 05:22:51
tags: 翻墙
comments: true
categories: 技术
---
本页面将详细演示如何在一台全新的Windows7电脑上架设起Chrome+XX_Net的上网渠道。

本文包含以下部分：

1. 下载和安装Chrome浏览器
2. 获取和运行XX-Net
<!-- more -->
3. 设置代理
4. 手动导入证书（备选）
5. 下载和安装Chrome浏览器

# 下载

[Chrome官网下载地址](https://www.google.cn/intl/zh-CN/chrome/browser/desktop/index.html)
虽然是CN网站，但是挂了"google"这个敏感词，所以会经常抽风。那么下面就多提供几个下载地址。

- 浏览迷网站：http://liulanmi.com/
- 新浪软件中心：http://tech.sina.com.cn/down/
- 卡饭chrome区：http://bbs.kafan.cn/forum-214-1.html

上面几个网站搜索或者点击chrome浏览器下载，建议用“Stable（稳定版）”

# 安装

为了不侮辱大家的智商，安装Chrome就不详解了，一路“确定”就ok了。

# 获取和运行XX-Net

- 打开[下载链接](https://github.com/XX-net/XX-Net/blob/master/code/default/download.md，选择稳定版下载)
<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112130952192?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
- 下载完毕后解压缩文件夹，运行文件夹中start.vbs文件 运行

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112122618591?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

- 如果弹出管理员权限请求（用户账户控制），请允许。

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112122703092?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>


- 首次运行可能会弹出防火墙警告，请允许访问。

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112122840017?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>


# 设置代理

## 方案一：简单方法

启动XX-Net后，右下角会出现托盘图标。右键单击托盘图标，点击“全局PAC智能代理”即可。 托盘右键菜单

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112123238206?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

## 方案二：安装和使用代理切换插件

- 打开XX-Net/SwitchyOmega文件夹；打开浏览器的扩展程序页面 chrome://extensions 。把SwitchyOmega.crx文件拖放到浏览器扩展程序页面安装。如图 
<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112123451895?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112123508351?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

- 添加扩展程序 SwitchyOmega

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112123554134?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>
- 跳过教程

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112123651635?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

- 导入bak文件 

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112123728823?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>



<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112123847491?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

- 点击从备份文件中恢复后，找到XX-Net/SwitchyOmega/OmegaOptions.bak文件，点击打开 bak文件

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112124536352?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

- 点击情景模式中的 XX-Net自动切换 ,跳过教程 教程

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112124624791?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

- 下拉点击“立即更新情景模式” 更新情景模式

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112124718291?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

- 点击SwitchyOmega，切换成“XX-Net自动切换”，如果使用的是X-Tunnel或SS，请点击“X-Tunnel自动切换”。 

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112124918745?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

- 到此，浏览器端设置代理也就完成了，还需最后一步，把XX-Net切换为“取消全局代理”，就可以畅游网络了。

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112124800588?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

# 手动导入证书（备选）

- 正常情况下，Chrome的证书都是自动导入的。手动导入证书，只是非正常情况下才会用到，比如遇到“您打开的链接不是私密连接”，这个时候就需要手动导入证书了。
- 点击浏览器 菜单-设置-下翻点击“显示高级设置”-点击“管理证书” 管理证书

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112125118512?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

- 选择“受信任的根证书颁发机构”这一栏，然后点击导入 导入证书 下一步

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112125210747?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>
<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112125246721?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>
- 点击浏览，然后定位到xx-net/data/gae_proxy文件夹，点击CA.crt文件，打开 
<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112125550905?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>
<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112125656398?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>


- 将证书存放在“受信任的根证书颁发机构”，点击下一步，完成 
<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112125352378?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

<div align=center>![这里写图片描述](http://img.blog.csdn.net/20170112125501270?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)</div>

到此手动导入证书也就完成了。
本文并非自己原创，[参考文献](https://github.com/XX-net/XX-Net/wiki/%E4%BD%BF%E7%94%A8Chrome%E6%B5%8F%E8%A7%88%E5%99%A8)

