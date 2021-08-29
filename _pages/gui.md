---
title: "Shuoyuan Wang - GUI for HAR"
layout: gridlay
excerpt: "Shuoyuan Wang -- GUI for HAR"
sitemap: false
permalink: /gui/
---

### GUI for Human Activity Recognition using wearable devices

<center>
<figure>
		<div id="projectid">
    <img src="{{ site.url }}{{ site.baseurl }}/images/explore/GUI.png" width="700px" />
		</div>

<figcaption>
<br>
Overview

</figcaption>
</figure>
</center>

- This project is a GUI based on Tkinter. The sensor datas operated by sliding window are stored in "/dataset/WISDM".The data can be download from <a href="https://www.cis.fordham.edu/wisdm/dataset.php">WISDM</a> website. We can extract random samples from them to predict human actions.
- The model in the Figure is algorithms based on machine learning or deep learning. We give the example of CNNs in our <a href="https://github.com/Claydon-Wang/GUI-for-HAR">respositories</a>. The model can be trained in remote server and further deployed on mobile devices like Raspberry Pi. Hence, we can intuitively evaluate the model efficiency through metrics such as inference time.
- The initial interface can be shown as below:

<center>
<figure>
		<div id="projectid">
    <img src="{{ site.url }}{{ site.baseurl }}/images/explore/origin.png" width="700px" />
		</div>

<figcaption>
<br>
Initial interface

</figcaption>
</figure>
</center>

- The results can be shown as below:

<center>
<figure>
		<div id="projectid">
    <img src="{{ site.url }}{{ site.baseurl }}/images/explore/classification.png" width="700px" />
		</div>

<figcaption>
<br>
Results example

</figcaption>
</figure>
</center>

#### Acknowledgements
Thank to my friend <a href="https://github.com/Chauncey-Wang">Xin Wang</a> for the discussion and help in this project.