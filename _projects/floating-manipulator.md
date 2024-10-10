---
title: "Object Capture for a Manipulator Subject to Floating-Base Disturbances"
collection: projects
topic: marine_robotics
toc: true
permalink: /projects/floating-manipulator/
abstract: "Research project I participated in at CUHK-Shenzhen, supervised by <a href='https://sse.cuhk.edu.cn/en/faculty/qianhuihuan'>Prof. QIAN Huihuan</a>, 2022 ~ 2023. In this project, I assisted a Ph.D. student in proposing and implementing a motion planning algorithm that allows a floating-base manipulator to capture objects under the disturbance of base motion." 
excerpt: "<img src='/images/projects/floating-manipulator/floating-manipulator.gif' width='700px'>"
date: 2023-03-08
---

{% include base_path %}
*Last updated on July 2024.*

---

## Introduction

This project was a research project I participated in at CUHK-Shenzhen, supervised by [Prof. QIAN Huihuan](https://sse.cuhk.edu.cn/en/faculty/qianhuihuan), 2022 ~ 2023. In this project, I assisted a Ph.D. student (now [Dr. XU Ruoyu](https://xuruoyuroy.github.io/)) in proposing and implementing a motion planning algorithm that allows a floating-base manipulator to capture objects under the disturbance of base motion.

![task](/images/projects/floating-manipulator/task.png)

## Relevant publication

For more technical details, please see our publication:
>R. Xu, **Z. Jiang**, B. Liu, Y. Wang, and H. Qian, "Confidence-Aware Object Capture for a Manipulator Subject to Floating-Base Disturbances," in _IEEE Transactions on Robotics (T-RO)_, vol. 40, pp.4396-4413, doi: [10.1109/TRO.2024.3463476](https://doi.org/10.1109/TRO.2024.3463476).

## Manipulator-assisted UAV landing on USV subject to wave disturbances

As illustrated in the figure above, this project originated from the need to **_use manipulators to assist UAVs in landing on USVs disturbed by waves_**. This is a beneficial feature for marine USV-UAV systems, especially when encountering bad weather and high see states.


![USV](/images/projects/floating-manipulator/usv.gif)

For more information about the USV-UAV system developed by our lab, you may refer to 
> R. Xu, C. Liu, Z. Cao, Y. Wang, and H. Qian, "A manipulator-assisted multiple UAV landing system for USV subject to disturbance", Ocean Engineering, vol. 299 (2024) 117306, doi: [10.1016/j.oceaneng.2024.117306](https://doi.org/10.1016/j.oceaneng.2024.117306).

For more information about the end effector used in this project, please see our [tethered landing system](/projects/tethered-landing/) project.