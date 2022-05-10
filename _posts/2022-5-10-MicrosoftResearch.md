---
layout: post
title: "Microsoft Research相关论文"
categories:
  - Motion Capture
tags:
  - Motion Capture
excerpt: Microsoft Research相关论文 以及一些相关的整理
comments: true

---

下面是Microsoft Research相关论文 以及一些相关的整理

# 一、 网站

## 1. [Human Pose Estimation for Kinect](https://www.microsoft.com/en-us/research/project/human-pose-estimation-for-kinect/)

### (1) [publications](https://www.microsoft.com/en-us/research/project/human-pose-estimation-for-kinect/publications/)

### (2) [human-pose-estimation](https://www.microsoft.com/en-us/research/search/?q=human-pose-estimation)

# 二、 一些文章

## 1. [Real-Time Human Pose Recognition in Parts from Single Depth Images](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=5995316)

(CVPR 2011    Microsoft Research Cambridge & Xbox Incubation)

### （1）流程图

![](https://wangchenjun521.github.io/assets/images/2022_05_10/001.png)

focus on localizing different body parts

将复杂的姿态估计问题，转化为更简单的每个像素的分类问题

### （2）效果图

![](https://wangchenjun521.github.io/assets/images/2022_05_10/002.png)

## 2. [Efficient regression of general-activity human poses from depth images](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6126270)

一种基于 Hough 森林从深度图像进行一般活动人体姿态估计的方法

 以多种方式扩展现有技术：多个 3D 关节的实时预测、投票权重的显式学习、投票压缩以允许更大的训练集，以及几个决策树训练目标的比较。 

工作的关键方面包括：**直接从原始深度图像回归，不使用任意中间表示**； 适用于一般运动（不限于特定活动）以及定位闭塞和可见身体关节的能力。

实验结果表明，我们的方法在几个数据集上产生了最先进的结果，包括具有挑战性的 MSRC-5000 姿态估计测试集，速度约为 **每秒200 帧** 。 轮廓的结果表明对其他成像方式具有更广泛的适用性。

指出了分割方法缺点：

      (a) 身体部分需要跟关节点大致对齐

      (b) 表面分割模式位于表面，而关节位于体内

      (c) 当相关部分被遮挡时，无法估计关节的位置。

方法：结合了下面两篇

 Class-specific ***Hough forests** for object detection. In PAMI. IEEE, 2009

 Human pose estimation with **implicit shape models**.




