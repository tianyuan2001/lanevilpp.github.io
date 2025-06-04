---
layout: home
title: LanEvil
subtitle: Benchmarking the Robustness of Autonomous Driving to Environmental Illusions: A Lane Perception Perspective
---

## Overview  

Environmental illusions (*e.g.*, shadows, reflections, and tire marks) are naturally existing yet overlooked phenomena in real-world driving environments. They can disturb visual perception, leading to misinterpretation of the scene and posing serious safety risks to autonomous driving (AD) systems. However, existing researches largely overlook these phenomena, leaving a critical gap.
To address this issue, we study AD robustness through the lane perception perspective, a fundamental task supporting core functions like cruise control and lane centering. We focus on two representative models: conventional lane detection (LD) and vision-language model-based systems (ADVLMs).
In this work, we introduce the first benchmark, *LanEvil++*, for evaluating the robustness of lane perception under environmental illusions. *LanEvil++* encompasses 14 types of illusions and leverages the CARLA simulator to generate 94 high-fidelity, fully controllable 3D scenes, yielding a dataset of 90,292 annotated images, 1,596 video clips, and 41,855 visual question answering pairs.
Extensive evaluations demonstrate that environmental illusions substantially degrade the performance of state-of-the-art LD methods. On average, LD models experience a 5.37% drop in Accuracy and a 10.70% decline in F1-score, while ADVLMs show a 1.89% reduction in GPT-score and a 0.66% drop in Language-score. Among all illusions, shadows emerge as the most disruptive factor, reducing accuracy by up to 7.39%. Furthermore, closed-loop simulations using OpenPilot and LMDrive reveal that these illusions can lead to incorrect driving decisions, underscoring their real-world implications. Complementary real-world case studies highlight safety-critical failures in actual traffic scenes. 
To enhance robustness, we propose the Multimodal Illusion Defense Approach (MIDA), which uses hard examples to improve illusion resistance. MIDA achieves substantial gains under challenging conditions, boosting robustness by 4.23% on LD models and 3.82% on ADVLMs. We hope this work brings greater attention to the threats posed by environmental illusions and motivates the development of more robust AD systems.

<!--<object data="/assets/img/framework_v2.pdf" type="application/pdf" > 
    <embed src="/assets/img/framework_v2.pdf"> 
    </embed> 
</object> -->

![](/assets/img/framework_gai.png)

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
<table border="0" style="max-width:100%; border-collapse: collapse; text-align:center; background: rgb(255, 255, 255);">
    <col align="center" width="50%">
    <col align="center"  width="50%">
    <tr>
        <th style="background: rgb(255, 255, 255);text-align:center; border: none">Original</th>
        <th style="background: rgb(255, 255, 255);text-align:center; border: none">Perturbed</th>
    </tr>
    <tr>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Rails/StraightAhead_Aside03_1_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Rails/StraightAhead_Aside03_1_alt38azm280.mp4" type="video/mp4">
            </video> 
        </td>
    </tr>
    <tr>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Rails/Uphill_Aside05_1_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Rails/Uphill_Aside05_1_alt30azm90.mp4" type="video/mp4"> 
            </video>
        </td>
    </tr>
    <tr>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Fence/StraightAhead_Grid03_1_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Shadow/Fence/StraightAhead_Grid03_1_alt9azm350.mp4" type="video/mp4"> 
            </video>
        </td>
    </tr>
    <tr>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Reflection/SunLight/Bend_t06_1_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Reflection/SunLight/Bend_t06_1_pd70alt10.mp4"> 
            </video>
        </td>
    </tr>
    <tr>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Reflection/StreetLight/StraightAhead_t03_2_wh_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/Reflection/StreetLight/StraightAhead_t03_2_wh_pd70.mp4"> 
            </video>
        </td>
    </tr>
    <tr>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/RoadInfrastructure/Fence/Turning_White01_1_ClearNoon_origin.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/RoadInfrastructure/Fence/Turning_White01_1_azm45alt30_fence.mp4"> 
            </video>
        </td>
    </tr>
    <tr>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/RoadInfrastructure/TireMarks/Turning_1_ClearNightInitial.mp4" type="video/mp4"> 
            </video>
        </td>
        <td style="background: rgb(255, 255, 255);border: none">
            <video controls autoplay loop muted width="100%">
                <source src="./assets/mp4s/RoadInfrastructure/TireMarks/Turning_1_ClearNight.mp4"> 
            </video>
        </td>
    </tr>
</table>
</div>
