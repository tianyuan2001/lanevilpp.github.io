---
layout: page
title: DataSet
subtitle: Detailed explanation of the dataset
---

## Dataset organization

Our *LanEvil* dataset contains two subsets, i.e., a training set with normal images and a test set with environmental illusions.

### *LanEvil* training set
<div style="column-count: 2">
  <div>
    <img src="assets/img/train.png">
  </div>

  <div>
    Due to the fact that not all cases that appear in the real world have environmental illusions, we use the training set consisting of <b>40,000</b> randomly sampled images to help model training.
  </div>
</div>


### *LanEvil* test set
<div style="column-count: 2">
  <div>
    <img src="assets/img/test.png">
  </div>
  <div>
    The test part consists of <b>50,292</b> images. For each basic environmental illusion, we provide an original case without any illusion and 2 - 10 perturbed cases, each consisting of 50 to 300 consecutively captured driving images.
  </div>
</div>

<br/>
<br/>

<!-- html div盒子 -->
<div style="column-count: 2">
  <div align=left>
    <img src="/assets/img/histogram_fig.png" width=400 heihgt=400>
    <div class=caption>
      The number of original and perturbed cases under four categories.
    </div>
  </div>
<br/>
  <div align=left>
    <img src="/assets/img/circle2-1.png" width=400 heihgt=400>
    <div class=caption>
      The case distribution of four illusion categories.
    </div>
  </div>
</div>
