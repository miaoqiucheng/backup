---
title: 边缘计算（Edge Computing）
date: 2017-03-09 09:06:34
tags: 学习
comments: true
categories: 技术
---
# 物联网体系结构

物联网作为一种技术体系，可以分为4层来看: 传感器（控制层）、网络层、平台以及应用层。

     传感控制层：感知和控制传输
	 网络层：数据传输
	 平台：作为通信、数据和管理
	 应用层：数据分析与相关应用的实际实施。 

平台与应用层应该是位于数据中心，其主要实现的功能应该包括管理、分析、控制和数据处理等等。网络层主要的功能则是进行数据传输以及通信。
	 <!-- more -->

# 为什么需要Edge computing
					
背景：

1. 云计算已经无法匹配海量数据处理
2. 从网络边缘到云数据中心网络带宽、延时的限制
3. 边缘设备涉及个人隐私与安全尤为明显
4. 能耗

很多行业对实时性、可靠性与安全性等有严格要求，而物联网作为一种便携可移动的装置，有其别与传统互联网设施的特点。---受限于接入带宽和流量以及成本、能耗等条件的限制，所以对数据应该进行合理的处理，特别是进行预处理，以便能够进行“物尽其用”，避免资源的浪费。因此，在靠近物或者数据源头的网络边缘就需要一个集连接、计算、存储和应用的开放平台，就近提供边缘智能服务。概括来说就是：边缘计算可以满足敏捷连接、实时业务、数据优化、应用智能、安全与隐私保护等方面的需求，而这些需求正是物联网行业需要解决的问题。

# 我理解的云计算与边缘计算

云计算：集中式大数据处理  
边缘计算：边缘式大数据处理

就像我们的手被火烧着（或者其他刺激）的时候，我们本能的收手，然后再将我们被火烧着了，并且感到了疼痛，及时的把手收起的过程传给大脑（边缘计算）。这个过程资源的消耗、信息的传输明显小于后者。而不是经过大脑，考虑我们是否感到疼痛，进而决定是否要进行收手（云计算）。边缘计算可以对一些简单的问题进行自行处理并将结果处理后的结果传输给云端。还有就是我认为边缘计算就是“微云”，云计算的缩小加持版本，靠近设备的小型数据中心。

# 边缘计算需要关注的四个方面

***<font color=#00ffff>1. Application</font>***


**Example:**

  Vehicular,Video surveillance,Smart city,Smart grid, Camera Intelligence,    Mobile and wearable,Disaster-relief,Bedside clinical.
								      
**Challenge:**

1. Real-time processing and communication
2. Security and privacy
3. Adaptive application development
4. Tools for the development and testing of apps in edge-computing
											   
***<font color=#00ffff>2. Architecture</font>***

**Challenge:** 

1. Enabiling QoS on Network Edge
2. Data Provenance
3. A Theorem for Tradeoffs,  
	(1)Mobility,(2)Latency,(3)Capability,(4)Privacy. The conflicts may be su     ch things as : large capability implies long latency and improving priv     acy dictates increasing latency
4. Cage-Level Securit

***<font color=#00ffff>3.Capability </font>***
***<font color=#00ffff>4.Service</font>***

**Questions：**

*1. What types of computing resources are there in edge computing?*

1. Edge devices(Smartphones, tablets, etc)
2. Backend clouds(Google Services, Facebook, etc)
3. Edge infrastructure(In-car servers that are built in a vehicle)

*2. Who provides the resources?*

1. Cloud service provider model
2. Hird party edge service provider model
3. End user model
	    
**Challenge:**

1. Naming, identifying, and discovering resources
2. Standardized APIs
3. Intelligent Edge Services
4. Security and Trust
5. Edge Service Ecosystem
			 
# Benefits

1. 分布式和低延时计算
2. 对终端设备的数据进行筛选，不必每条原始数据都传送到云，充分利用设备的空闲资源，在边缘节点处过滤和分析。节能省时。
3. 减缓数据爆炸，网络流量的压力，在进行云端传输时通过边缘节点进行一部分简单数据处理，进而能够设备响应时间，减少从设备到云端的数据流量。
4. 智能化（Edge intelligence）

# Requests

1. 差异性、可扩展性、隔离性、可靠性
2. 众多的设备要怎样部署
3. 服务模式会有何种变化
4. 不能所有数据都在边缘节点计算亦不能所有数据都在云端进行计算，如何进行数据筛选，对实时、简单的数据进行处理，而将一些数据传输云端
5. 轻量级库和算法
6. 可持续能源消耗
7. 高水准的服务质量（QoS）和服务体验（QoE）
8. 开放和安全的使用边缘节点
9. 微型操作系统和虚拟化

写于2017.3.9

