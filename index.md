---
layout: home
title: LanEvil
subtitle: Benchmarking the Robustness of Lane Detection to Environmental Illusions
---

## Overview  

For the first time, we study the potential threats caused by environmental illusions to LD(lane detection) and establishes the first comprehensive benchmark *LaneEvil* for evaluating the robustness of LD against the natural corruption. We systematically design 14 common but critical environmental illusion types (e.g., shadow, reflection) by rigorously analyzing the influence factors in LD tasks; according to the real-world environment, we then establish 94 realistic and editable 3D cases using the commonly used CARLA simulator, yielding the dataset with 90,292 sampled dataset images. We conducted large-scale experiments and benchmarked the robustness of widely used LD methods on *LaneEvil*, where we observed strong performance degeneration (-5.37% Accuracy and -10.70% F1-Score on average) underscoring the severe safety threats. In addition, we also test commercial auto-driving systems OpenPilot and Apollo via collaborative simulation, where our perturbed cases could cause incorrect decisions resulting in traffic accidents. We hope our works can contribute to advancing more robust auto-driving systems in the future.

![](/assets/img/framework.png)

## Dataset Examples

![](/assets/img/RoadDamage.png)

---

![](/assets/img/TrafficObstruction.png)

---



## Challenges

<video width="800" height="450" controls autoplay loop muted>     <source src="./assets/video/openPilot.mp4" type="video/mp4"> </video>
