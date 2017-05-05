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

<video id="video" width="100%" controls="" preload="none" poster="http://omjk76pbk.bkt.clouddn.com/rocblog/post/xbot-project/xbot-poster-1.png">
      <source id="mp4" src="http://198.46.242.227/video/xbot-3D.mp4" type="video/mp4">
      <p>Your user agent does not support the HTML5 Video element.</p>
</video>

## 办公室场景
机器人已实现在办公室场景下的**同步定位与建图**的功能,视频中,机器人从办公室(中科院软件所四号楼一层办公区)的任意位置启动之后,激光雷达扫描机器人周围非盲区范围内的障碍物并建图.

这里,尽管激光雷达是支持360度全范围内的扫描,但是由于机器人的构造与安装因素的影响,我们所获取的范围大概在300度左右,这也已经比市面上大多数机器人的平均扫描范围270度大了,因而足够满足需求.

视频中机器人逐渐在我们给的几个探测目标点的指引下探测了一大片办公室区域,最后,我们让机器人在已探测的区域当中自主规划路径和导航,成功到达机器人的起始位置.

<video id="video" width="100%" controls="" preload="none" poster="http://omjk76pbk.bkt.clouddn.com/rocblog/post/xbot-project/xbot-poster-2.png">
      <source id="mp4" src="http://198.46.242.227/video/xlab401-merge.mp4" type="video/mp4">
      <p>Your user agent does not support the HTML5 Video element.</p>
</video>
## 软件博物馆讲解
软件博物馆讲解的视频拍摄在中科院软件所五号楼一层的软件博物馆,也是中国第一个以计算机软件为展示出内容的博物馆,博物馆从上世纪最初的计算机打孔编程,一直讲到现在的计算机高级编程技术.其中,还展出了像庞大的容量仅仅几KB的存储设备等类似的很多有意思的玩意儿.

让机器人带领游客参观软件博物馆,并且同步讲解每一处的展出内容,这是我们机器人实际应用实例之一.视频中,机器人从博物馆门口,通过对游客的人脸识别之后致相应的欢迎词.定点运动规划一条固定路径,带着游客慢慢参观展览,最终完成一次循环后回到博物馆门口,等待下一位游客的到来.
<video id="video" width="100%" controls="" preload="none" poster="http://omjk76pbk.bkt.clouddn.com/rocblog/post/xbot-project/xbot-poster-3.png">
      <source id="mp4" src="http://198.46.242.227/video/xbot_museum_face.mp4" type="video/mp4">      
</video>

软件博物馆中的机器人,DIY自带低音炮.
![博物馆中的机器人](http://omjk76pbk.bkt.clouddn.com/rocblog/post/xbot-project/IMG_3707.JPG)

机器人正在带领几名小学生参观软件博物馆,不得不说小学生们太调皮了,有时候还将机器人围得水泄不通!
![](http://omjk76pbk.bkt.clouddn.com/rocblog/post/xbot-project/IMG_3708.JPG)

老师正在给学生们讲解机器人的原理,不是我哈,是我领导.
![](http://omjk76pbk.bkt.clouddn.com/rocblog/post/xbot-project/IMG_3709.JPG)
