---
title: 'CodeVIO: Visual-Inertial Odometry with Learned Optimizable Dense Depth'
authors:
  - admin
  - Nathaniel Merrill
  - Wei Li
  - Yong Liu
  - Marc Pollefeys
  - Guoquan Huang
date: '2021-05-01'
publication_types: ['paper-conference']
publication: 'IEEE International Conference on Robotics and Automation (ICRA), Best Paper Award Finalist in Robot Vision'
publication_short: 'ICRA 2021'
abstract: 'We present a lightweight, tightly-coupled deep depth network and visual-inertial odometry (VIO) system, which can provide accurate state estimates and dense depth maps of the immediate surroundings. Leveraging the proposed lightweight Conditional Variational Autoencoder (CVAE) for depth inference and encoding, we provide the network with previously marginalized sparse features from VIO to increase the accuracy of initial depth prediction and generalization capability. The compact encoded depth maps are then updated jointly with navigation states in a sliding window estimator in order to provide the dense local scene geometry. Our full system exhibits state-of-the-art pose estimation accuracy and can run in real-time with single-thread execution while utilizing GPU acceleration only for the network and code Jacobian.'
tags: [VIO, Dense Depth, Deep Learning]
featured: true
links:
  - name: arXiv
    url: 'https://arxiv.org/abs/2012.10133'
url_code: ''
---
