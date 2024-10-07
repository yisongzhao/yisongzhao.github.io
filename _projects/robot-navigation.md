---
title: "Mobile Robot Navigation Using Vision and LiDAR"
collection: projects
topic: others
permalink: /projects/robot-navigation/
abstract: "Course project (ECE4310 Programming for Robotics, Spring 2022) at CUHK-Shenzhen. In this project, I programmed a mobile robot to perform an auto-delivery task in the Gazebo simulator. I used vision data to implement global path planning and LiDAR data to implement local path planning and obstacle avoidance. "
excerpt: "<img src='/images/projects/robot-navigation/navigation.gif' width='700px'>"
toc: true
date: 2022-04-12
---

{% include base_path %}
*Last updated on April 2022.*

---

## Introduction
This project was a course project of ***ECE4310 Programming for Robotics, Spring 2022***, at CUHK-Shenzhen. In this project, I programmed a service robot to perform an auto-delivery task in the Gazebo simulator. The robot is required to traverse all delivery stations in a room while avoiding obstacles. Each station is identified by an AR-tag, which also encodes the location of the next station relative to the current station, as described in the following figure.

![task](/images/projects/robot-navigation/task.png)

## Method
I implemented the robot's navigation algorithm based on the [ROS Navigation Stack](https://github.com/ros-planning/navigation). I used vision data to implement global path planning and LiDAR data to implement local path planning and obstacle avoidance. 


## For more info

You may check the [project report](/files/pdf/ECE4310%20Project%201%20Report%20(119010130).pdf) for more technical details. 

## Demonstration

Here is a video demo of this project.

<video controls style="width: 100%; height: auto;" controlsList="nodownload" oncontextmenu="return false;" preload="auto">
  <source src="/files/webm/navigation.webm" type="video/webm">
  Your browser does not support the video tag.
</video>