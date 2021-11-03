---
title: 计算机网络复习（二）--物理层
subtitle: 计算机网络复习

# Summary for listings and search engines
summary: 计算机网络第二章内容复习 --物理层


# Date published
date: "2021-11-02T00:00:00Z"

# Date updated
lastmod: "2021-11-02T00:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: '[**Arcaea**]'
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

## 重点

1. 物理层的任务：确定与传输媒体的接口的一些特性
2. 常用的信道复用技术
3. 常用的宽带接入技术？


## 内容
 
1. 与传输媒体的接口的一些特性：
    - 机械特性：接线器的形状、尺寸
    - 电气特性：电压范围
    - 功能特性：某一电平的电压的意义
    - 过程特性：可能时间的出现顺序
2. 信号分类：模拟信号（连续信号）、数字信号（离散信号）
3. 信道
    - 单向通信：又称**单工通信**
    - 双向交替通信：又称**半双工通信**
    - 双向同时通信：又称**全双工通信**
4. 基带信号：来自信源的信号
5.  基带信号-》基带信号：基带调制（编码）
    基带信号-》模拟（带通）信号：使用载波，带通调制

6. 常用编码：
    - 不归零制
    - 归零制
    - 曼彻斯特：中心向上代表0或1
    - 差分曼彻斯特：开始边界跳变代表0，不变代表1

7. 带通调制
    - 调幅
    - 调频
    - 调相

* 正交振幅调制QAM:一个码元4bit
* 【S=BlogN  S:比特率,B:波特率,N:码元状态数】

8. 信道的极限容量：
    - 奈氏准则：不考虑噪声，带宽W,码元最大传输速率2W
    - 信噪比：信噪比（dB）=10lg(S/N) (dB)   【此处S/N为信号平均功率/噪声平均功率】 
    - 香农公式:信道极限传输速率C=Wlog(1+S/N)  【W:带宽，S/N:信噪比】

9. 传输媒体（略）

10. 信道复用
     - 频分复用FDM:同样时间占用不同带宽资源
     - 时分复用TDM:每个信号在每个TDM帧中占用固定序号的时隙 （同步时分复用）
         - 统计时分复用STDM:使用STDM帧来传送复用的数据，各用户有了数据就随时发往集中器的输入缓存，集中器按序扫描后放入STDM帧中，帧满发送 （异步时分复用）
     - 波分复用WDM:光的频分复用,一根光纤同时传输多个频率接近的光载波信号
         - 密集波分复用DWDM：一根光纤复用几十路光载波信号
     - 码分复用CDM:各用户使用不同码型。在CDMA（码分多址）中，一个比特时间被分为m个短间隔成为码片。