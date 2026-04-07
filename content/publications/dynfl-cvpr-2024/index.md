---
title: 'Dynamic LiDAR Re-simulation using Compositional Neural Fields'
authors:
  - Hanfeng Wu
  - admin
  - Stefan Leutenegger
  - Or Litany
  - Konrad Schindler
  - Shengyu Huang
date: '2024-06-01'
publication_types: ['paper-conference']
publication: 'IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), Highlight'
publication_short: 'CVPR 2024 Highlight'
abstract: 'We introduce DyNFL, a novel neural field-based approach for high-fidelity re-simulation of LiDAR scans in dynamic driving scenes. DyNFL processes LiDAR measurements from dynamic environments, accompanied by bounding boxes of moving objects, to construct an editable neural field. This field, comprising separately reconstructed static background and dynamic objects, allows users to modify viewpoints, adjust object positions, and seamlessly add or remove objects in the re-simulated scene. A key innovation of our method is the neural field composition technique, which effectively integrates reconstructed neural assets from various scenes through a ray drop test, accounting for occlusions and transparent surfaces. Our evaluation with both synthetic and real-world environments demonstrates that DyNFL substantially improves dynamic scene LiDAR simulation, offering a combination of physical fidelity and flexible editing capabilities.'
tags: [LiDAR, Neural Fields, Simulation]
featured: true
links:
  - name: arXiv
    url: 'https://arxiv.org/abs/2312.05247'
url_code: 'https://github.com/prs-eth/Dynamic-LiDAR-Resimulation'
---
