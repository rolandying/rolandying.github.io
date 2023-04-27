---
layout: page
title: FusionLane
description: High-precision map construction for Autopilot
img: assets/img/p1.jpg
importance: 1
category: research
---

HIGH-PRECISION could not only provide high-precision positioning based on map matching, but also disclose complex information about roads and pavements as a priori knowledge for unmanned vehicles, for example, lane limits, slope, curvature, heading, etc. High-precision maps can be seen as a complementary element of the perception module of unmanned vehicles, and they help unmanned vehicles focus on other tasks such as detection and tracking of moving obstacles. To enable autonomous operation, the high-precision lane level map must therefore contain accurate lane marking information.


<div class="row justify-content-sm-center">
    <div class="col-8">
        {% include figure.html path="assets/img/p1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Compared to camera data, which suffers from lower accuracy and distortion-related issues, LiDAR point cloud data can better fulfill precision requirements.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}

You can display .mp4 files and embeded YouTube links as well

<div class="row justify-content-sm-center">
    <div class="col-6">
        {% include figure.html path="https://www.youtube.com/embed/dQw4w9WgXcQ" title="Rickroll" class="embed-responsive embed-responsive-16by9 img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
	Never click on unfamiliar links.
</div>
