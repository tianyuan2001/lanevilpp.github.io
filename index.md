---
layout: home
title: LanEvil
subtitle: Benchmarking the Robustness of Lane Detection to Environmental Illusions
---

## Overview  

For the first time, we study the potential threats caused by environmental illusions to LD(lane detection) and establishes the first comprehensive benchmark *LaneEvil* for evaluating the robustness of LD against the natural corruption. We systematically design 14 common but critical environmental illusion types (e.g., shadow, reflection) by rigorously analyzing the influence factors in LD tasks; according to the real-world environment, we then establish 94 realistic and editable 3D cases using the commonly used CARLA simulator, yielding the dataset with 90,292 sampled dataset images. We conducted large-scale experiments and benchmarked the robustness of widely used LD methods on *LaneEvil*, where we observed strong performance degeneration (-5.37% Accuracy and -10.70% F1-Score on average) underscoring the severe safety threats. In addition, we also test commercial auto-driving systems OpenPilot and Apollo via collaborative simulation, where our perturbed cases could cause incorrect decisions resulting in traffic accidents. We hope our works can contribute to advancing more robust auto-driving systems in the future.

<!--<object data="/assets/img/framework_v2.pdf" type="application/pdf" > 
    <embed src="/assets/img/framework_v2.pdf"> 
    </embed> 
</object> -->

![](/assets/img/framework.png)

## Dataset Examples

![](/assets/img/RoadDamage.png)

---

![](/assets/img/TrafficObstruction.png)

---

![](/assets/img/Shadow.png)

---

![](/assets/img/Reflection.png)

## Challenges

Here we exhibit the video results of lane detecion by <a href="https://github.com/Wolfwjs/GANet">GANet</a>(ResNet-18). The green lines in left column are predicted in original scenes while the red lines in right column are predicted in perturbed scenes.

The first three rows represent **Shadow** illusion. Row 4 and 5 represent **Reflection** illusion. The last two rows represent **RoadDamage** illusion.

<div>
<table border="0" style="max-width:100%; border-collapse: collapse; text-align:center;">
    <col align="center" width="50%">
    <col align="center"  width="50%">
    <tr>
        <th style="text-align:center; border: none">Original</th>
        <th style="text-align:center; border: none">Perturbed</th>
    </tr>
    <tr>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Rails/StraightAhead_Aside03_1_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Rails/StraightAhead_Aside03_1_alt38azm280.mp4" type="video/mp4">
            </video> 
        </td>
    </tr>
    <tr>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Rails/Uphill_Aside05_1_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Rails/Uphill_Aside05_1_alt30azm90.mp4" type="video/mp4"> 
            </video>
        </td>
    </tr>
    <tr>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Fence/StraightAhead_Grid03_1_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Fence/StraightAhead_Grid03_1_alt9azm350.mp4" type="video/mp4"> 
            </video>
        </td>
    </tr>
    <tr>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Reflection/SunLight/Bend_t06_1_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Reflection/SunLight/Bend_t06_1_pd70alt10.mp4"> 
            </video>
        </td>
    </tr>
    <tr>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Reflection/StreetLight/StraightAhead_t03_2_wh_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Reflection/StreetLight/StraightAhead_t03_2_wh_pd70.mp4"> 
            </video>
        </td>
    </tr>
    <tr>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/RoadInfrastructure/Fence/Turning_White01_1_azm45alt30_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/RoadInfrastructure/Fence/Turning_White01_1_azm45alt30_fence.mp4"> 
            </video>
        </td>
    </tr>
    <tr>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/RoadInfrastructure/TireMarks/Turning_1_ClearNightInitial.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/RoadInfrastructure/TireMarks/Turning_1_ClearNight.mp4"> 
            </video>
        </td>
    </tr>
</table>
</div>

<div style="text-align:center;">
<span id="busuanzi_container_site_pv"> 
	LaneEvil has been visited <span id="busuanzi_value_site_pv"></span> times.
</span>
</div>