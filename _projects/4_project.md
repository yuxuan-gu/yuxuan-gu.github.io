---
layout: page
title: Self-balancing maze-solving rover
description: 
img: assets/img/Rover/Rover-3.png
importance: 1
category: 2023
# related_publications: true
---

# Project information:
- **Category**: Summer term project
- **Year**: 2023
- **Location**: Imperial College London, London, UK

Collaborating as a team of 2 EEE and 4 EIE members, we designed a self-balancing rover proficient in autonomously solving mazes, live mapping, and finding the shortest paths.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Rover/Rover-3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Rover/Rover-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Rover traversing the maze
</div>

The rover integrates NEMA 17 stepper motors, A4988 drivers, an MPU-6050 gyroscope, ESP32, FPGA, and a camera. Employing FPGA vision technology, we achieved superior image processing, ensuring precise navigation and obstacle detection. Our approach includes PID, triangulation, A*, clustering, and graph theory algorithms, finely tuned to optimize performance and effectiveness.

<div class="row">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Rover/Rover-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Rover/Rover-4.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, fontend overview of the system. Right, PID controller for stepper motors.
</div>

