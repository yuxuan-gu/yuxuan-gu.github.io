---
layout: page
title: Remote Control of Colour-tracking Robotic Arm
description: 
img: assets/img/Robotic-arm/robotic_arm1.png
importance: 1
category: 2023
# related_publications: true
---

# Project information:
- **Category**: Undergraduate Research Opportunities Programme (UROP) [[Github Link](https://github.com/guyuxuan9/UROP_robotic_arm)]
- **Year**: 2023
- **Supervisor**: Prof.Thomas Parisini and Dr. Kaiwen Chen
- **Location**: Imperial College London, London, UK

I developed a 4-DOF robotic arm with color-tracking capabilities, utilizing remote control within the ROS2 framework. This project integrated a USB camera as a sensor within the feedback loop to effectively manage bus servo motors.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Robotic-arm/robotic_arm1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Composition of the robotic arm
</div>

Geometric inverse kinematics analysis was employed to calculate joint variables based on end-effector position and orientation. To control the motors, a Raspberry Pi was employed to transmit commands through UART while simultaneously publishing image frames to ROS2 topics. Additionally, I implemented controller separation on a remote machine, allowing communication with the local node through the ROS2 network, and subsequently conducted an in-depth analysis of stability margins. Furthermore, I built a 2nd order transfer function model by exploring the step response of one of the motors.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Robotic-arm/robotic_arm3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Robotic-arm/robotic_arm2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, utilisation factor of a station in a week is shown. Right, predicted and ground truth utilisation rate.
</div>

