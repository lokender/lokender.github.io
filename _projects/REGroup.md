---
layout: page
shorttitle: REGroup [Robust Classification]
title: REGroup - Rank-aggregating Ensemble of Generative Classifiers for Robust Predictions
description: In IEEE Winter Conference on Applications of Computer Vision (<b>WACV</b>), 2022
img: assets/img/REGroup.png
importance: 2
category: work
github: https://github.com/lokender/REGroup
---

**Authors:** [Lokender Tiwari](https://lokender.github.io/)<sup>1,2</sup>, &nbsp;
[Anish Madan](https://scholar.google.com/citations?user=eZ4WZmIAAAAJ&hl=en)<sup>1</sup>, &nbsp;
[Saket Anand](https://www.iiitd.edu.in/~anands/index.html)<sup>1</sup>, &nbsp;
[Subhasis Banerjee](http://www.cse.iitd.ac.in/~suban//)<sup>3,4</sup>

**Affiliations:** <sup>1</sup>[IIIT-Delhi](https://www.iiitd.ac.in/), &nbsp;
<sup>2</sup>[TCS Research](https://www.tcs.com/tcs-research), &nbsp;
<sup>3</sup>[IIT-Delhi](https://home.iitd.ac.in/), &nbsp;
<sup>4</sup>[Department of Computer Science, Ashoka University](https://www.ashoka.edu.in/computerscience)

**Links:** [PDF](https://openaccess.thecvf.com/content/WACV2022/papers/Tiwari_REGroup_Rank-Aggregating_Ensemble_of_Generative_Classifiers_for_Robust_Predictions_WACV_2022_paper.pdf), &nbsp;
[Conference Talk](https://youtu.be/hwKjcc1IJqw), &nbsp;
[Conference Talk Slides](/assets/pdf/REGroup_talk_PPT.pdf), &nbsp;
[Poster](/assets/pdf/REGroup_poster.pdf), &nbsp;
[Code](https://github.com/lokender/REGroup) &nbsp;


<hr>

## Abstract
> Deep Neural Networks (DNNs) are often criticized for being susceptible to adversarial attacks. Most successful defense strategies adopt adversarial training or random input transformations that typically require retraining or fine-tuning the model to achieve reasonable performance. In this work, our investigations of intermediate representations of a pre-trained DNN lead to an interesting discovery pointing to intrinsic robustness to adversarial attacks. We find that we can learn a generative classifier by statistically characterizing the neural response of an intermediate layer to clean training samples. The predictions of multiple such intermediate-layer based classifiers, when aggregated, show unexpected robustness to adversarial attacks. Specifically, we devise an ensemble of these generative classifiers that rank-aggregates their predictions via a Borda count-based consensus. Our proposed approach uses a subset of the clean training data and a pre-trained model, and yet is agnostic to network architectures or the adversarial attack generation method. We show extensive experiments to establish that our defense strategy achieves state-of-the-art performance on the ImageNet validation set. 


<div class="row justify-content-md-center">
    <div class="col-md-auto">
        {% include figure.html path="assets/img/REGroup_teaser.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <h6 style="text-align:center"> <b>Figure 1:</b> REGroup Overview. </h6>
    
</div>

<div class="row justify-content-md-center">
    <div class="col-md-auto">
        <iframe display="block" width="640" height="320" src="https://www.youtube.com/embed/hwKjcc1IJqw?autoplay=1"> </iframe> 
    </div> 
</div>
<div class="caption">
    <h6 style="text-align:center"> <b>WACV 2022 Conference Talk</b></h6>
</div>




<hr>
<h3 style="text-align:center"> <b> Sample Results</b> </h3>

<div class="row">
    <div class="col-sm">
        {% include figure.html path="assets/img/regroup_eg_1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm">
        {% include figure.html path="assets/img/regroup_eg_2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<!-- <div class="caption">
    <h6 style="text-align:center"> <b>Figure 2:</b> Qualitative depth evaluation results on KITTI Odometry test set. Improvement in depth prediction of farther scene points. </h6>
</div> -->

&nbsp;

<div class="row justify-content-md-center">
    <div class="col-md-8">
        {% include figure.html path="assets/img/regroup_eg_3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<!-- <div class="caption">
    <h6 style="text-align:center"> <b>Figure 3:</b> Qualitative depth evaluation results on KITTI Raw Eigen split test set. MonoDepth2-M is the MonoDepth2 model trained using monocular images. </h6>
</div> -->


<hr>

<h4>Bibtex</h4>
<pre>@inproceedings{tiwari2022regroup,
  title={REGroup: Rank-aggregating Ensemble of Generative Classifiers for Robust Predictions},
  author={Tiwari, Lokender and Madan, Anish and Anand, Saket and Banerjee, Subhashis},
  booktitle={Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision},
  pages={2595--2604},
  year={2022}
}
</pre>
