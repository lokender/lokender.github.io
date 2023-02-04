---
layout: page
shorttitle: Pseudo RGB-D SLAM
title: Pseudo RGB-D for Self-Improving Monocular SLAM and Depth Prediction
description: In European Conference on Computer Vision (<b>ECCV</b>), 2020
img: assets/img/self_improving_framework.png
importance: 1
category: work
---

**Authors:** [Lokender Tiwari](https://lokender.github.io/)<sup>1</sup>, &nbsp;
[Pan Ji](https://sites.google.com/site/peterji1990)<sup>2</sup>, &nbsp;
[Quoc-Huy Tran](https://cs.adelaide.edu.au/~huy/home.php)<sup>2</sup>, &nbsp;
[Bingbing Zhuang](https://bbzh.github.io/)<sup>2</sup>, &nbsp;
[Saket Anand](https://www.iiitd.edu.in/~anands/index.html)<sup>1</sup>, &nbsp;
[Manmohan Chandraker](https://cseweb.ucsd.edu/~mkchandraker/)<sup>2,3</sup>

**Affiliations:** <sup>1</sup>[IIIT-Delhi](https://www.iiitd.ac.in/), &nbsp;
<sup>2</sup>[NEC Labs America, Inc.](http://www.nec-labs.com/research-departments/media-analytics/media-analytics-home), &nbsp;
<sup>3</sup>[UCSD](https://ucsd.edu/)

**Links:** [PDF](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560426.pdf), &nbsp;
[arXiv](https://arxiv.org/pdf/2004.10681), &nbsp;
[Conference Talk and Demos](https://www.youtube.com/watch?v=N9Di1uN0ut0&list=PL-cvWulnEGU6gBmgr8leVbJ6k7aI3MTjA), &nbsp;
[Conference Talk Slides](/assets/pdf/pRGBD_ECCV_Main_Talk.pdf), &nbsp;
[Demo Talk Slides](/assets/pdf/pRGBD_ECCV_Demo_Talk.pdf), &nbsp;


<hr>

## Abstract
> Classical monocular Simultaneous Localization And Mapping (SLAM) and the recently emerging convolutional neural networks (CNNs) for monocular depth prediction represent two largely disjoint approaches towards building a 3D map of the surrounding environment. In this paper, we demonstrate that the coupling of these two by leveraging the strengths of each mitigates the others shortcomings. Specifically, we propose a joint narrow and wide baseline based self-improving framework, where on the one hand the CNN-predicted depth is leveraged to perform pseudo RGB-D feature-based SLAM, leading to better accuracy and robustness than the monocular RGB SLAM baseline. On the other hand, the bundleadjusted 3D scene structures and camera poses from the more principled geometric SLAM are injected back into the depth network through novel wide baseline losses proposed for improving the depth prediction network, which then continues to contribute towards better pose and 3D structure estimation in the next iteration. We emphasize that our framework only requires unlabeled monocular videos in both training and inference stages, and yet is able to outperform state-of-the-art self-supervised monocular and stereo depth prediction networks (e.g., Monodepth2) and feature-based monocular SLAM system (i.e., ORB-SLAM). Extensive experiments on KITTI and TUM RGB-D datasets verify the superiority of our self-improving geometry-CNN framework.


<div class="row justify-content-md-center">
    <div class="col-md-auto">
        {% include figure.html path="assets/img/self_improving_framework.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <h6 style="text-align:center"> <b>Figure 1:</b> A SELF-SUPERVISED, SELF-IMPROVING FRAMEWORK -- It alternates between pose refinement (blue arrows) and depth refinement (red arrows). </h6>
    
</div>

<div class="row justify-content-md-center">
    <div class="col-md-auto">
        <iframe display="block" width="640" height="320" src="https://www.youtube.com/embed/N9Di1uN0ut0?autoplay=1"> </iframe> 
    </div>
</div>
<div class="caption">
    <h6 style="text-align:center"> <b>ECCV 2020 Conference Talk</b></h6>
</div>




<hr>
<h3 style="text-align:center"> <b>ECCV 2020 Demo Track : RGB vs Pseudo RGB-D SLAM and Monocular Depth Prediction Demos</b> </h3>


<div class="row justify-content-md-center">
    <div class="col-md-auto">
        <iframe display="block" width="640" height="320" src="https://www.youtube.com/embed/gdY4yn0J4E0?autoplay=1"> </iframe> 
    </div>
</div>
<div class="caption">
    <h6 style="text-align:center"> <b>Video 1:</b> KITTI Odometry Sequence 19 </h6>
</div>

<div class="row justify-content-md-center">
    <div class="col-md-auto">
        <iframe display="block" width="640" height="320" src="https://www.youtube.com/embed/OOPJpHexrdE?autoplay=1"> </iframe> 
    </div>
</div>
<div class="caption">
    <h6 style="text-align:center"> <b>Video 2:</b> KITTI Odometry Sequence 11 </h6>
</div>


<div class="row justify-content-md-center">
    <div class="col-md-auto">
        <iframe display="block" width="640" height="320" src="https://www.youtube.com/embed/MffXsKjy9W0?autoplay=1"> </iframe> 
    </div>
</div>
<div class="caption">
    <h6 style="text-align:center"> <b>Video 3:</b> TUM RGB-D Sequence freiburg3 Large Cabinet Validation. </h6>
</div>

<hr>
<h3 style="text-align:center"> <b>Results: Qualitative Depth Estimation</b> </h3>

<div class="row justify-content-md-center">
    <div class="col-md-auto">
        {% include figure.html path="assets/img/qual_depth_far.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <h6 style="text-align:center"> <b>Figure 2:</b> Qualitative depth evaluation results on KITTI Odometry test set. Improvement in depth prediction of farther scene points. </h6>
</div>

&nbsp;

<div class="row justify-content-md-center">
    <div class="col-md-auto">
        {% include figure.html path="assets/img/qual_depth.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <h6 style="text-align:center"> <b>Figure 3:</b> Qualitative depth evaluation results on KITTI Raw Eigen split test set. MonoDepth2-M is the MonoDepth2 model trained using monocular images. </h6>
</div>
<hr>
<h3 style="text-align:center"> <b>Results: Qualitative Pose Estimation Results</b> </h3>
<div class="row justify-content-md-center">
    <div class="col-md-auto">
        {% include figure.html path="assets/img/qual_pose_kitti.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <h6 style="text-align:center"> <b>Figure 4:</b> Qualitative pose evaluation results on KITTI Odometry sequences. </h6>
</div>

<hr>

<h4>Bibtex</h4>
<pre>@inproceedings{tiwari2020pseudo,
    author={Tiwari, Lokender and Ji, Pan and Tran, Quoc-Huy and Zhuang, Bingbing and Anand, Saket 
    and Chandraker, Manmohan},
    title     = {Pseudo RGB-D for Self-Improving Monocular SLAM and Depth Prediction}, 
    booktitle = {European Conference on Computer Vision},
    year      = {2020}
}
</pre>
