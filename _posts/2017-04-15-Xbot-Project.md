---
layout:     post
title:      "xbot机器人项目"
subtitle:   "xbot机器人组,让机器人学会走路."
date:       2017-04-15 15:32:00
author:     "Roc"
header-img: "img/post/xbot-project.png"
catalog: true
tags:
    - 机器人
---

>xbot机器人组的使命:让机器人学会走路!

## 小组成立

xbot机器人小组成立于2016年1月,成立之初,小组属于中国科学院软件研究所总体部的先导组.2016年7月,小组正式转到协同创新中心,作为中心的一个前沿研究分支.

xbot机器人小组最初成立的目标是,实现移动机器人室内自主运动和导航,使机器人在室内环境下能在够任意点之间运动.
之后随着多个研究项目的入驻,小组逐渐调整和整合机器人的功能,以适应各类定制环境下的需求.

室内移动机器人在现实中很多方面都有着广泛的应用,包括:
* 家庭陪护
* 医疗辅助
* 商场导购
* 酒店迎宾
* 学校教育
* 会议管理

至今,xbot机器人小组的研究成果分别在:
* 办公室
* 博物馆

两个场景得到了成功的落地和应用.

## 初步仿真效果

2016年6月,室内办公室场景下的xbot运动和导航的仿真效果和初步实际运动效果已成功实现.为增强视觉效果,我在ROS的rviz工具的基础之上特添加了
三维的环境地图.根据办公室的实际场景,通过3dmax三维效果实现软件构建了xbot的3D地图,在视觉效果层面
增加了机器人运行的带入感.

具体实现效果视频使用2x倍速播放,整个环境3D地图由软件初始化过程中预先加载.位置变动性不大的障碍物如办公室桌子,墙壁,柱子以及门窗等我们
将其视为固定障碍物,由地图预先加载;而像椅子,花盆,茶几之类的位置变动性较大的障碍物我们使用动态障碍物加载的方式加入地图,在程序运行过程中支持随时
加入突然出现的障碍物.

<iframe height=498 width=510 src='http://player.youku.com/embed/XMjcxMzA1MzYyMA==' frameborder=0 'allowfullscreen'></iframe>

## 办公室场景

<iframe height=498 width=510 src='http://player.youku.com/embed/XMjcxMzA1Nzk1Mg==' frameborder=0 'allowfullscreen'></iframe>

## 软件博物馆讲解

<iframe height=498 width=510 src='http://player.youku.com/embed/XMjcxMzA2MzIxMg==' frameborder=0 'allowfullscreen'></iframe>


![](http://omjk76pbk.bkt.clouddn.com/rocblog/post/xbot-project/IMG_3707.JPG)
![](http://omjk76pbk.bkt.clouddn.com/rocblog/post/xbot-project/IMG_3708.JPG)
![](http://omjk76pbk.bkt.clouddn.com/rocblog/post/xbot-project/IMG_3709.JPG)
