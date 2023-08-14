---
layout: post
title:  "Semantic SLAM Project"
date:   2023-04-28
excerpt: "University of Michigan, EECS568 | Python, Semantic SLAM"
project: true
tag:
- SemanticSLAM
- Python
- project
comments: true
---

•	Report about Semantic SLAM: `LiDAR Fusion and Dynamic Object Masking for ORB-SLAM2` [(Read More)](../assets/reports/LiDAR_Fusion_and_Dynamic_Object_Masking_for_ORB_SLAM2.pdf)

•	In this study, we presented a modification to ORB-SLAM2 model, to improve its performance in dynamic environments. We integrated a depth prediction sensor-fusion
model to better understande the distances of object in the environment, and a 3D object detection algorithm to identify key objects and remove the negative effects by dynamic objects/remain the static objects to achieve a better result using ORB-SLAM2.

•	During this teamwork, I mainly responsible for writing Python code and implement the depth prediction using Data Fusion. The depth map can be generated using LiDAR point clouds and RGB monocular image as data provided from [KITTI dataset](https://www.cvlibs.net/datasets/kitti/eval_odometry.php). Compared to the camera trajectory using only monocular images, the trajectory generated using depth map (contain data fusion of two sources) performed a better result (0.456 for Monocular+DP, 2.54 for Monocular Only, in RMSE).