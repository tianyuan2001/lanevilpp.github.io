---
layout: page
title: DataSet
subtitle: Detailed explanation of the dataset
---

## Dataset organization

Our *LanEvil* dataset contains two subsets, i.e., a training set with normal images and a test set with environmental illusions. Due to the fact that not all cases that appear in the real world have environmental illusions, we use the training set consisting of **40,000** randomly sampled images to help model training.  The test part consists of **50,292** images. For each basic environmental illusion, we provide an original case without any illusion and 2 - 10 perturbed cases, each consisting of 50 to 300 consecutively captured driving images.

<!-- html div盒子 -->
<!--
<div style="column-count: 2">
  <div align=left>
    <img src="/assets/img/histogram_fig.png">
    </img>
  </div>
<br/>
  <div align=left>
    <img src="/assets/img/circle2-1.png">
    </img>
  </div>
</div>
-->

<div>
<table border="0" style="max-width:100%; border-collapse: collapse; text-align:center; border: none">
    <col align="center" width="50%" style="border: none">
    <col align="center"  width="50%" style="border: none">
    <tr style="border: none; background: none">
        <th style="text-align:center; border: none">
        The number of original and perturbed cases.</th>
        <th style="text-align:center; border: none">
        The case distribution of four illusion categories.
        </th>
    </tr>
    <tr style="border: none; background: none">
        <td style="border: none">
            <img src="/assets/img/histogram_fig.png" width="100%"/>
        </td>
        <td style="border: none">
            <img src="/assets/img/circle2-1.png" width="100%"/>
        </td>
    </tr>
</table>
</div>



