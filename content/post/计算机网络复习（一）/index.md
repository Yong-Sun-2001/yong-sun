---
title: 计算机网络复习（一）
subtitle: 计算机网络复习

# Summary for listings and search engines
summary: 计算机网络第一章内容复习 

# Link this post with a project
projects: []

# Date published
date: "2021-11-1T00:00:00Z"

# Date updated
lastmod: "2021-11-1T00:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**图片来源url**](https://unsplash.com/photos/szrJ3wjzOMg)'
  focal_point: ""
  placement: 2
  preview_only: false

authors:
- Yong Sun

tags:
- Yong Sun
- 计算机网络

categories:
- 计算机网络
---

## Overview

1. **概述**
2. 重点：1）计算机网络性能指标 2）互联网边缘部分和核心部分的作用 3）分层次的体系结构


## Content
 
1. 互联网两个重要基本特点：**连通性**，**共享**
2. 
  - 边缘部分：所有连接在互联网上的主机，用来通信和资源共享；通信方式划分：客户-服务器方式（C/S），对等方式（P2P）
  - 核心部分：大量网络和连接这些网络的路由器，为边缘部分提供连通性和交换。路由器：分组交换（存储转发技术）
3. 
  - 电路交换：整个报文比特流连续地从源点直达终点，需要预先分配传输带宽，适合连续传送大量数据
  - 报文交换：整个报文先传送到相邻节点，全部存储下来后查找转发表，不需要预先分配传输带宽，适合传送突发数据
  - 分组交换：单个分组传送到相邻节点，存储下后查找转发表，不需要预先分配传输带宽，适合传送突发数据，比报文交换时延小，灵活性更好

4. 网络类别
   - WAN:广域网,几十到几千km
   - MAN:城域网,5-50km
   - LAN:局域网，1km
   - PAN:个人区域网，10m

   - 公用网
   - 专用网

5. 网络的性能指标
  - 速率
  - 带宽
  - 吞吐量
  - 时延
  - 时延带宽积
  - 往返时间RRT
  - 利用率

6. 网络的非性能特征
  - 费用
  - 质量
  - 标准化
  - 可靠性
  - 可拓展性、可升级性
  - 易于管理维护

7. 网络协议由三要素:语法、语义、同步

8. 体系结构
  - OSI/RM : 7层 （应用层、表示层、会话层、运输层、网络层、数据链路层、物理层）
  - TCP/IP ：4层 （应用层、运输层、网际层IP、链路层）
  - 五层的体系结构：应用层、运输层、网络层、数据链路层、物理层
