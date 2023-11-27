---
layout: page
title: Experiments
subtitle: Detailed results of the experiments
---

## Evaluation results of 5 LD models 

### Average results

Table1 shows the average results of 4 illusion categroies. The first 4 LD modeles use Resnet-18 while SCNN uses VGG. The bold values represent the minimum in each column, and “Gap” is computed by “Perturbed” minus “Original”.

<div>
<table border="0" style="max-width:100%; border-collapse: collapse; text-align:center; background: rgba(0, 0, 0, 0);">
    <col align="center" width="100%">
    <tr style="border: none">
        <th style="text-align:center; border: none">Table 1. The evaluation results of 4 illusion categories (%).</th>
    </tr>
    <tr style="border: none">
        <td style="text-align:center;border: none">
            (a) Accuracy results (%).
            <img src="/assets/img/acc.png">
        </td>
    </tr>
    <tr style="border: none">
        <td style="text-align:center;border: none">
            (b) F1-score results (%).
            <img src="/assets/img/f1.png">
        </td>
    </tr>
</table>
</div>


### Breakdown results

Here we show the breakdown results of 14 illusion types.
Table 2 shows the breakdown results in Accuracy and F1-score drop.

<div>
<table border="0" style="max-width:100%; border-collapse: collapse; text-align:center; background: rgba(0, 0, 0, 0);">
    <col align="center" width="100%">
    <tr style="border: none">
        <th style="text-align:center; border: none">Table 2. The breakdown results of each illusion type in Accuracy and F1-score drop (%).</th>
    </tr>
    <tr style="border: none">
        <td style="text-align:center;border: none">
            (a) Accuracy drop (%).
            <img src="/assets/img/acc_drop.png">
        </td>
    </tr>
    <tr style="border: none">
        <td style="text-align:center;border: none">
            (b) F1-score drop (%).
            <img src="/assets/img/f1_drop.png">
        </td>
    </tr>
</table>
</div>

Table 3 shows the breakdown Accuracy results under original scenes and perturbed scenes.

<div>
<table border="0" style="max-width:100%; border-collapse: collapse; text-align:center; background: rgba(0, 0, 0, 0);">
    <col align="center" width="100%">
    <tr style="border: none">
        <th style="text-align:center; border: none">Table 3. The breakdown Accuracy results of each illusion type under original scenes and perturbed scenes (%).</th>
    </tr>
    <tr style="border: none">
        <td style="text-align:center;border: none">
            (a) Accuracy under original scenes (%).
            <img src="/assets/img/acc_original.png">
        </td>
    </tr>
    <tr style="border: none">
        <td style="text-align:center;border: none">
            (b) Accuracy under perturbed scenes (%).
            <img src="/assets/img/acc_perturbed.png">
        </td>
    </tr>
</table>
</div>

Table 4 shows the breakdown F1-score results under original scenes and perturbed scenes.

<div>
<table border="0" style="max-width:100%; border-collapse: collapse; text-align:center; background: rgba(0, 0, 0, 0);">
    <col align="center" width="100%">
    <tr style="border: none">
        <th style="text-align:center; border: none">Table 4. The breakdown F1-score results of each illusion type under original scenes and perturbed scenes (%).</th>
    </tr>
    <tr style="border: none">
        <td style="text-align:center;border: none">
            (a) F1-score under original scenes (%).
            <img src="/assets/img/f1_original.png">
        </td>
    </tr>
    <tr style="border: none">
        <td style="text-align:center;border: none">
            (b) F1-score under perturbed scenes (%).
            <img src="/assets/img/f1_perturbed.png">
        </td>
    </tr>
</table>
</div>

## Evaluation results of 5 severity levels

Figure 1 shows the Accuracy drop of various models using ResNet-18 backbone (SCNN uses VGG backbone) across different severity levels under 4 illusion categories.

<div>
<table border="0" style="max-width:100%; border-collapse: collapse; text-align:center; background: rgba(0, 0, 0, 0);">
    <col align="center" width="33%">
    <col align="center" width="33%">
    <col align="center" width="33%">
    <tr style="border: none">
        <td style="text-align:center;border: none">
            <img src="/assets/img/ganet-final_exp_res18_s8.png">
            (a) GANet
        </td>
        <td style="text-align:center;border: none">
            <img src="/assets/img/ganet-final_exp_res18_s8.png">
            (b) BezierLaneNet
        </td>
        <td style="text-align:center;border: none">
            <img src="/assets/img/ganet-final_exp_res18_s8.png">
            (c) LaneATT
        </td>
    </tr>
</table>
</div>

<div>
<table border="0" style="max-width:100%; border-collapse: collapse; text-align:center; background: rgba(0, 0, 0, 0);">
    <col align="center" width="17%">
    <col align="center" width="33%">
    <col align="center" width="33%">
    <col align="center" width="17%">
    <tr style="border: none">
        <td style="text-align:center;border: none">
        </td>
        <td style="text-align:center;border: none">
            <img src="/assets/img/SCNN-vgg16.png">
            (d) SCNN.
        </td>
        <td style="text-align:center;border: none">
            <img src="/assets/img/SCNN-vgg16.png">
            (e) UFLD.
        </td>
        <td style="text-align:center;border: none">
        </td>
    </tr>
</table>
</div>
<div>
<table border="0" style="max-width:100%; border-collapse: collapse; text-align:center; background: rgba(0, 0, 0, 0);">
    <col align="center" width="100%">
    <tr style="border: none">
        <th style="text-align:center; border: none">
        Figure 1. Accuracy drop across 5 severity levels(%).
        </th>
    </tr>
</table>
</div>