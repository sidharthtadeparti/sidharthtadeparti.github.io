---
layout: page
title: Automotive Control.
description: Non-linear model predictive control for Heavy-vehicle platooning.
img: assets/img/Platooning/PlatoonModel2.JPG
importance: 2
category: major
---

This project represents a year-long effort towards my bachelor's thesis at IIT Madras. I worked at the automotive control lab toward developing model predictive controllers for heavy vehicle applications.

A platoon consists of several trucks moving together at high speeds with a small inter-vehicular spacing. In such formations, a trade-off exists between energy efficiency and stability that depends on the spacing.

<b>The research objective is therefore to design controllers that offer both stable and efficienct performance while utilizing a detailed vehicle dynamics model.</b>

The project makes use of two approaches, a centralized approach and a distributed approach and contrasts their performance. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Platooning/PlatoonModel2.JPG" title="Centralized Control" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A schematic of the centralized control framework.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Platooning/PlatoonModelDist.JPG" title="Centralized Control" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A schematic of the distributed control framework.
</div>

The above frameworks have been tested under different road friction conditions to understand their generality. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Platooning/VeloctyTracking_0.4_AC" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Platooning/VeloctyTracking_0.8.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Platooning/DC2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
Controller performance on acceleration, deceleration and drive cycle manoevres respectively. 
</div>

Finally, co-simulation was used to test the controller performance on a harware-in loop setup.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Platooning/HiL_Setup.JPG" title="Centralized Control" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Schematic of the HiL setup.
</div>


A detailed description can be found <a="https://ieeexplore.ieee.org/document/10178412" >here</a>