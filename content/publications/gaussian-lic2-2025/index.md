---
title: 'Gaussian-LIC2: LiDAR-Inertial-Camera Gaussian Splatting SLAM'
authors:
  - Xiaolei Lang
  - Jiajun Lv
  - Kai Tang
  - Laijian Li
  - Jianxin Huang
  - Lina Liu
  - Yong Liu
  - admin
date: '2025-07-01'
publication_types: ['preprint']
publication: 'arXiv preprint arXiv:2507.04004'
publication_short: 'arXiv 2025'
abstract: 'This paper presents the first photo-realistic LiDAR-Inertial-Camera Gaussian Splatting SLAM system that simultaneously addresses visual quality, geometric accuracy, and real-time performance. The proposed method performs robust and accurate pose estimation within a continuous-time trajectory optimization framework, while incrementally reconstructing a 3D Gaussian map using camera and LiDAR data, all in real time. To effectively address under-reconstruction in regions not covered by the LiDAR, we employ a lightweight zero-shot depth model that synergistically combines RGB appearance cues with sparse LiDAR measurements to generate dense depth maps, enabling reliable Gaussian initialization in LiDAR-blind areas. We also explore how the incrementally reconstructed Gaussian map can improve the robustness of odometry by tightly incorporating photometric constraints from the Gaussian map into the continuous-time factor graph optimization.'
tags: [SLAM, Gaussian Splatting, LiDAR]
featured: false
links:
  - name: arXiv
    url: 'https://arxiv.org/abs/2507.04004'
url_code: 'https://github.com/APRIL-ZJU/Gaussian-LIC'
---
