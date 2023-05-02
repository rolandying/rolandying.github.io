---
layout: page
title: Peg-in-hole assembly
description: Robotic grasping & high-precision peg-in-hole assembly task
img: assets/img/p2.jpg
importance: 2
category: LUT
---

Since 2020, I have been pursuing a doctoral degree at the Intelligent Machinery Laborato-ry within the Department of Mechanical Engineering at LUT University in Finland. My su-pervisor is Prof. Huapeng Wu.We are involved in the overarching research initiative known as ITER (International Ther-monuclear Experimental Reactor). Our primary responsibility lies in the remote handling maintenance operations within the reactor's vacuum chamber.

The environment within the reactor's vacuum chamber is considerably more challenging than ordinary settings, primarily due to its construction from smooth metallic materials. Depth cameras or LiDAR struggle to provide accurate observations in such conditions. Consequently, we need to implement various automated maintenance operations in the absence of reliable three-dimensional data.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pj21.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pj22.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The compare between the observation data of LIDAR(left) and camera(right) sensor on smooth metallic object.
</div>

My specific research focus comprises two components: robotic grasping and high-precision rigid peg-in-hole assembly.These investigations were conducted in environments that closely mimic the highly challenging conditions of a reactor's vacuum chamber. By employing multi-sensor fusion and leveraging deep reinforcement learning, we ultimately succeeded in effectively accomplishing the related tasks.In my first research task, robotic grasping, we adopted a conservative yet reliable ap-proach by combining deep learning and traditional computer vision algorithms. This strate-gy effectively mitigated the propagation of uncertainty from three-dimensional sensor ob-servations to control commands, resulting in stable and satisfactory grasping outcomes.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pj23.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The strucure of muti-sensor based peg-in-hole assembly method.
</div>

Following the robotic grasping task, we delved into high-precision rigid peg-in-hole assembly. In this study, the gap between the axis and hole was less than 0.1 millimeters (even lower than the repeatability accuracy of the UR10 robot we utilized), with a certain degree of randomness in the relative position between the end-effector and the grasped axis. To address these challenges, we fused data from a monocular camera and force sensors, employing deep reinforcement learning to train the robotic arm to execute assembly operations in a manner akin to human hand-eye coordination. This approach ultimately yielded excellent results. Some of the experiments is shown in the video.

<div class="row justify-content-sm-center">
    <div class="col-10">
        {% include figure.html path="https://www.youtube.com/embed/Vna5jrJm85I" title="Peg-in-hole" class="embed-responsive embed-responsive-16by9 img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
	The Robotic Grasping and peg-in-hole assembly experiment.
</div>

More details could be found in the corresponding publlications:

1.[RGB-D-Based Robotic Grasping in Fusion Application Environments](https://www.mdpi.com/2076-3417/12/15/7573)

2.[Mastering Autonomous Assembly in Fusion Application with Learning-by-doing: a Peg-in-hole Study](https://arxiv.org/abs/2208.11737)

