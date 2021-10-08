---
title: "Shuoyuan Wang - MIA"
layout: gridlay
excerpt: "Shuoyuan Wang -- MIA"
sitemap: false
permalink: /MIA/
---

### 1. Not End-to-End: Explore Multi-Stage Architecture for Online Surgical Phase Recognition. <a href="https://arxiv.org/abs/2107.04810">paper link</a>

#### 1.1 Why Not End-to-End？
-  Refinement stage uses the output of predictor stage as input, so the performance of prediction is very important. Although you can achieve low error rate on trainset, which can be refined for better performance, base model will certainly make mistakes on the testset and make no sense to refinement (refining the error cannot boost performance.
- If we use the end-to-end strategy, the limited size of current datasets for surgery phase recognition cannot afford the refinement stage with additional parameters, which leads to overfitting on testset.


#### 1.2 Aims and Solutions
To simulate the real output of the predictor by generating two disturbed sequences. 
- Mask-Hard-Frame: Using their former techniques to find hard frames in trainset, which are not recognizable from their visual appearance, and cover the hard frames via a black mask. As is shown in Figure.1, frame-wise methods may perform poorly.
- Cross-Validate: Through Cross Validate, the valset can play the role of testset, the output can be simulated as the real predictions of the predictor.

<center>
<figure>
		<div id="projectid">
    <img src="{{ site.url }}{{ site.baseurl }}/images/explore/MIA/1.png" width="700px" />
		</div>

<figcaption>
<br>
hard frame in visual appearance

</figcaption>
</figure>
</center>

#### 1.3 Experiment Reproduction
I both use their pretrained model and local trained model. The performance of local based model and refinement model may higher than they report in manuscript.

<center>
<figure>
		<div id="projectid">
    <img src="{{ site.url }}{{ site.baseurl }}/images/explore/MIA/NETE.png" width="700px" />
		</div>

<figcaption>
<br>
Result on cholec80

</figcaption>
</figure>
</center>