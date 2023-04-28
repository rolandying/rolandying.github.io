---
layout: page
title: Robotic pick-and-place
description: A monocular camera-based robotic pick-and-place method
img: assets/img/p3.jpg
importance: 3
category: LUT
---



Throughout the previous researches, we experienced the drawbacks of reinforcement learning, such as the potential collision risks and time-consuming training. These insights prompted us to leverage simulation environments to accelerate agent training in our subsequent robotic pick-and-place research. In this research, we capitalized on the ability of reinforcement learning to optimize temporal differences (TD) error and recover three-dimensional spatial information from two-dimensional images. This allowed us to achieve robotic pick-and-place operations using only a monocular camera. 

<div class="row">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/p3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/pj31.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A sub-environment in the simulator(left) and the monocular camera data used in our method(right)
</div>

Of course, there are some regrets in this research, such as not being able to validate the performance of the model in real-world environments due to time constraints. Sloving the sim-to-real gap is our next step research, we believe that the accessibility of the input data and the efficient distributed training of multiple sub-environments will facilitate its transfer to a realistic environment. The training process is shown in the video.

<div class="row justify-content-sm-center">
    <div class="col-10">
        {% include figure.html path="https://www.youtube.com/embed/z-LApEu1-hw" title="Peg-in-hole" class="embed-responsive embed-responsive-16by9 img-fluid rounded z-depth-1" %}
    </div>
</div>

More details could be found in the corresponding publlication: [Monocular Camera-Based Robotic Pick-and-Place in Fusion Applications](https://www.mdpi.com/2076-3417/13/7/4487).