---
title: 'Coco-LIC: Continuous-Time Tightly-Coupled LiDAR-Inertial-Camera Odometry using Non-Uniform B-spline'
authors:
  - Xiaolei Lang
  - Chao Chen
  - Kai Tang
  - Yukai Ma
  - Jiajun Lv
  - Yong Liu
  - admin
date: '2023-09-01'
publication_types: ['article-journal']
publication: 'IEEE Robotics and Automation Letters (RA-L)'
publication_short: 'RA-L 2023'
abstract: 'We propose an efficient continuous-time LiDAR-Inertial-Camera Odometry, utilizing non-uniform B-splines to tightly couple measurements from the LiDAR, IMU, and camera. In contrast to uniform B-spline-based continuous-time methods, our non-uniform B-spline approach offers significant advantages in terms of achieving real-time efficiency and high accuracy by dynamically and adaptively placing control points, taking into account the varying dynamics of the motion. To enable efficient fusion of heterogeneous LiDAR-Inertial-Camera data within a short sliding-window optimization, we assign depth to visual pixels using corresponding map points from a global LiDAR map, and formulate frame-to-map reprojection factors for the associated pixels. Our LiDAR-Inertial-Camera odometry system is extensively evaluated on both challenging scenarios with sensor degenerations and large-scale scenarios, and has shown comparable or higher accuracy than the state-of-the-art methods.'
tags: [LiDAR, SLAM, Continuous-Time]
featured: false
links:
  - name: arXiv
    url: 'https://arxiv.org/abs/2309.09808'
url_code: 'https://github.com/APRIL-ZJU/Coco-LIC'
---
