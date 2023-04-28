---
layout: page
title: FusionLane
description: High-precision map construction for Autopilot
img: assets/img/publication_preview/FL.jpg
importance: 1
category: USTC
---

High-precision map could not only provide high-precision positioning based on map matching, but also disclose complex information about roads and pavements as a priori knowledge for unmanned vehicles, for example, lane limits, slope, curvature, heading, etc. High-precision maps can be seen as a complementary element of the perception module of unmanned vehicles, and they help unmanned vehicles focus on other tasks such as detection and tracking of moving obstacles. To enable autonomous operation, the high-precision lane level map must therefore contain accurate lane marking information.


<div class="row justify-content-sm-center">
    <div class="col-8">
        {% include figure.html path="assets/img/p1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Compared to camera data, which suffers from lower accuracy and distortion-related issues, LiDAR point cloud data can better fulfill precision requirements.
</div>

The picture above is the top view of two consecutive frames of data in the KITTI dataset collected by a camera (upper row) and LIDAR (lower row, we convert the reflection intensity information into RGB information). As can be seen, the distortion of the point cloud data is significantly smaller. Meanwhile, the  high-precision maps does not require real-time online construction. Thus, We first use [Deeplab](https://arxiv.org/abs/1706.05587v3) to semantically segment the top view of the camera, and then use its segmentation results as input to assist in the semantic segmentation of the point cloud data. Our network structure is illustrated as blow.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/publication_preview/FL.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Network structure of FusionLane.
</div>

This method for effective semantic segmentation of the LIDAR points cloud bird’s eye view (LBEV) by introducing classification information of visual images was first proposed by this study. Experiments show that our method could achieve accurate and  high-quality results for sparse LBEV semantic segmentation. More details could be found in the [paper](/publications/).

