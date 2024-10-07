---
title: "Object Sorting Using Eye-in-Hand Manipulator"
collection: projects
topic: others
permalink: /projects/object-sorting/
abstract: "Course project (ECE4310 Programming for Robotics, Spring 2022) at CUHK-Shenzhen. In this project, I programmed a 6-DoF eye-in-hand manipulator to perform an object sorting task: place blocks into buckets of the same color as them. "
excerpt: "<img src='/images/projects/object-sorting/sorting.gif' width='700px'>"
toc: true
date: 2022-04-13
---

{% include base_path %}
*Last updated on April 2022.*

---

## Introduction
This project was a course project of ***ECE4310 Programming for Robotics, Spring 2022***, at CUHK-Shenzhen. In this project, I programmed a 6-DoF serial manipulator ([Interbotix WidowX 250](https://www.trossenrobotics.com/widowx-250)) with eye-in-hand camera
configuration to perform an intelligent sorting task: automatically places the different colored
blocks into the corresponding colored buckets. 

![setup](/images/projects/object-sorting/setup.png)

## Method

In this project, I used the [ROS MoveIt!](https://moveit.ros.org/) toolkit to implement most of the functions, including motion planning and obstacle avoidance. I used the [OpenCV](https://opencv.org/) library to implement a HSV mask based method to detect and distinguish the differently colored targets. 

![hsv](/images/projects/object-sorting/hsv.png)

I used linear regression for single pose eye-in-hand calibration (the robot is programmed to recognize objects using the camera only in a preset pose. Therefore, only the preset pose need to be calibrated). 


$$\begin{bmatrix}x_{w}\\y_{w}\end{bmatrix} = \boldsymbol{k}^{\top} \begin{bmatrix}x_{c}\\y_{c}\end{bmatrix} + \boldsymbol{b}$$

Where $[x_{w}, y_{w}, 0]^{\top}$ is target's position in world frame, and $[x_{c}, y_{c}]^{\top}$ is target's position in camera image frame. In this project, coefficients $\boldsymbol{k}$ and $\boldsymbol{b}$ were computed by using least squares on multiple pairs of sampled target positions. 

## For more info

You may check the [project report](/files/pdf/ECE4310%20Project%202%20Report%20(119010130).pdf) for more technical details. 

## Demo

Here is a video demo of this project.

{% include base_path %}

<!-- <div style="position: relative; padding-bottom: 56.25%; height: 0;">
  <iframe src="/files/sorting.mp4" style="position: absolute; width: 100%; height: 100%; border: none;" sandbox="" allowfullscreen></iframe>
</div> -->

<video controls style="width: 100%; height: auto;" controlsList="nodownload" oncontextmenu="return false;" preload="auto">
  <source src="/files/webm/sorting.webm" type="video/webm">
  Your browser does not support the video tag.
</video>