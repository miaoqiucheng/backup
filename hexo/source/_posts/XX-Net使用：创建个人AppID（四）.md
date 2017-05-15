---
title: XX-Net使用：创建个人AppID（四）
date: 2017-02-08 05:29:02
tags: 翻墙
category: 技术
comments: true
---
## 登录Google帐户

https://www.google.com/ncr (若无帐户，需注册，若注册失败，可能需要更换线路或梯子---[蓝灯VPN下载点击这里，多平台使用](https://github.com/getlantern/forum/issues/833))

<!--more-->

## 创建AppID

1. 打开https://console.developers.google.com ，左击顶部Project，然后左击创建项目
![1-CreateProject.png](http://img.blog.csdn.net/20170328131415853?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
2. 输入项目名称后，会自动帮你匹配可用ID，然后左击创建(请细读此教程底部说明)
	![2-CreateProject.png](http://img.blog.csdn.net/20170328131427197?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

## 设置AppID的App引擎

1. 打开https://console.cloud.google.com/home/ (Google Cloud Platform)，可在左上角选择对应AppID
2. 在页面顶端中部搜索栏输入App 引擎回车进入App引擎管理界面
在弹出的“欢迎使用App引擎”界面的左侧点击选择一种语言，选择Python (解决方案最先源于https://github.com/XX-net/XX-Net/issues/4720)
在“你想在哪里提供自己的应用？”界面，更改选择位置为us-central
以上方法为老方法,

**因GAE升级，设置AppID的App引擎需要用新的方法**

1. 进入 https://console.cloud.google.com/start ，点击 Project 、创建项目，记下您的项目id，点击创建。
![default](http://img.blog.csdn.net/20170328131457083?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
2. 点击搜索框右边的按钮激活云端shell，页面底部会出现黑底白字，输入 gcloud config set project 23333 ，将前面的23333替换为您的项目id ，按下键盘的enter键，然后输入 gcloud beta app create --region us-central ，再按一次enter。

3. 当底部出现 Success! The app is now created. Please use 'gcloud app deploy' to deploy your first app. 时，创建appid成功。此时可以重复前面两步，创建更多的appid

## 部署服务端

1. 打开XX-Net的设置页：http://127.0.0.1:8085 ，切换到部署服务端
2. 输入AppID后，左击开始部署，会弹出授权窗口
![3-Deploy.png](http://img.blog.csdn.net/20170328131522651?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
3. 左击Allow，然后就会进行服务端的部署
![4-RequestForPermission.png](http://img.blog.csdn.net/20170328131535995?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
4. 部署完成后，切换到配置，输入部署好的AppID后左击保存
![5-Config.png](http://img.blog.csdn.net/20170328131546745?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
5. 切换到***状态***来确认状态
![6-Status.png](http://img.blog.csdn.net/20170328131558522?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbWlhb3FpdWNoZW5n/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

## 说明

- 每个AppID每天1G流量，一般每个Google帐户最多12个AppID.
- AppID的数量只影响流量，不影响速度.
	 
本文并非原创，[参考内容.](https://github.com/XX-net/XX-Net/wiki/how-to-create-my-appids)

