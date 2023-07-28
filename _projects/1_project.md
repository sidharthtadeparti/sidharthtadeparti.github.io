---
layout: page
title: Motion Planning of a Surgical Robot
description: Sampling-based planning for a 7 DoF Manipulator.
img: assets/img/IRRT_Star_Constraint.gif
importance: 1
category: major
---
This project was completed as a part of an introductory course on motion planning offered by IIT Madras. The broad goal was to apply motion planning technique to surgical robotics.

<b> The problem statement:</b>

<i>Plan and simulate the motion of the end effector of a 7-DoF Kuka iiwa manipulator while adhering to a remote center of motion (RCM) constraint.<\i>

The RCM constraint helps ensure that the needle only moves vertically and rotates about the insertion point. This ensures that the skin is not stretched during surgery.

The manipulator used is very high dimensional and hence the conventional graph based plannign algorithms are intractable for such a problem. Sampling based technquies such as RRT and its many variants are used to plan the path. A major challenge arises from the RCM constraint itself, with a highly restricted and narrow sampling space. 

In this project, all components except the simulation package for the robot are engineered from scratch. The forward kinematics and collision check modules are developed using the geometric properties of the robot. The final path is simulated using Gazebo.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MotionPlanning/RRT_Constraint.gif" title="RRT" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MotionPlanning/RRT_Star_Constraint.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MotionPlanning/IRRT_Star_Constraint.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The above animations depict the performance of RRT RRT* and IRRT* respectively on the planning problem. The differences are delineated in the report.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MotionPlanning/Workflow.JPG" title="Flow of Information" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The setup of the implementation is depicted by the above flow chart.
</div>

To learn more about the project, please refer the <a href='https://github.com/sidt36/ED5215-Path-Planning-Project---RCM'>Github Repository</a>.


