---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: hero
    id: about
    content:
      title: |
        Robotics Cognition
        and Learning Group
      text: |
        We are part of the Robotics Department at **MBZUAI**, Abu Dhabi, UAE. Our research vision is to enable natural interaction and seamless collaboration between robots and humans in open environments by accurately understanding robot states, surrounding 3D scenes, and action execution.
      primary_action:
        text: Join Our Team
        url: '/opportunities'
        icon: hero/user-group
      secondary_action:
        text: View Publications
        url: '#publications'
        icon: hero/academic-cap
      announcement:
        text: "We are hiring PhD students, research assistants, and postdocs!"
        link:
          text: "Learn more"
          url: "/opportunities"
    design:
      css_class: ""
      background:
        gradient_mesh:
          enable: true
          style: "waves"
          animation: "pulse"
          intensity: "medium"
          colors:
            - "primary-500/30"
            - "blue-600/20"
            - "indigo-600/15"

  - block: research-areas
    id: research-areas
    content:
      title: Research Focus Areas
      subtitle: ''
      text: ''
      # TODO: Update the research areas below to reflect the group's actual focus
      items:
        - name: Robot Perception & State Estimation
          description: Developing robust multi-sensor fusion algorithms (LiDAR-Inertial-Camera) for accurate robot localization and mapping in challenging environments
          icon: hero/eye
          gradient: from-blue-400 to-indigo-600
          status: active
          topics:
            - Visual-Inertial Odometry
            - LiDAR SLAM
            - Multi-Sensor Fusion
            - Continuous-Time Estimation
          cta:
            text: Learn More
            url: /research/robot-perception

        - name: 3D Vision & Spatial AI
          description: Advancing 3D scene understanding through neural radiance fields, Gaussian splatting, and foundation model integration for holistic scene representation
          icon: hero/cube-transparent
          gradient: from-purple-400 to-pink-600
          status: active
          topics:
            - Neural Radiance Fields (NeRF)
            - 3D Gaussian Splatting
            - Dense 3D Reconstruction
            - Open-Vocabulary 3D Understanding
          cta:
            text: Learn More
            url: /research/3d-vision

        - name: Embodied AI & Human-Robot Interaction
          description: Enabling robots to understand, interact with, and manipulate objects in open environments through vision-language-action models and hand-object interaction
          icon: hero/hand-raised
          gradient: from-green-400 to-emerald-600
          status: active
          topics:
            - Hand-Object Interaction
            - Mobile Manipulation
            - Vision-Language-Action (VLA)
            - Visual Language Navigation (VLN)
          cta:
            text: Learn More
            url: /research/embodied-ai
    design:
      layout: cards
      css_class: "bg-gradient-to-b from-gray-50 to-white dark:from-gray-900 dark:to-gray-800"
      spacing:
        padding: ["5rem", 0, "5rem", 0]

  - block: team-showcase
    id: team
    content:
      title: Team
      subtitle: ''
      text: ''
      user_groups:
        - Principal Investigators
        - Postdoctoral Researchers
        - PhD Students
        - Research Assistants
        - Visiting Students
      sort_by: 'Params.last_name'
      sort_ascending: true
      cta:
        text: View All Members
        url: /authors
        icon: user-group
    design:
      show_role: true
      show_organizations: false
      show_interests: true
      show_social: true
      css_class: "bg-gray-50 dark:bg-gray-900"
      spacing:
        padding: ["3rem", 0, "3rem", 0]

  - block: collection
    id: publications
    content:
      title: Recent Publications
      text: 'Find the full publication list on [Google Scholar](https://scholar.google.com/citations?user=CePv8agAAAAJ).'
      filters:
        folders:
          - publications
        exclude_featured: false
      count: 5
    design:
      view: citation

  - block: collection
    id: news
    content:
      title: News
      subtitle: ''
      text: ''
      page_type: blog
      count: 5
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      offset: 0
      order: desc
    design:
      view: card
      columns: 1

  - block: contact-info
    id: contact
    content:
      title: Contact
      subtitle: ''
      address:
        lines:
          - Robotics Cognition and Learning (RCL) Group
          - Robotics Department
          - Mohamed bin Zayed University of Artificial Intelligence (MBZUAI)
          - Masdar City, Abu Dhabi, UAE
      office_hours:
        - "Sunday - Thursday: 9:00 AM - 5:00 PM (UAE time)"
      email: xingxing.zuo@mbzuai.ac.ae
      social:
        - icon: brands/google-scholar
          url: https://scholar.google.com/citations?user=CePv8agAAAAJ
        - icon: brands/github
          url: https://github.com/ZuoJiaxing
      prospective:
        title: Prospective Members
        text: We are always looking for motivated PhD students, research assistants, visiting students, and postdocs to join the group.
        button:
          text: View Open Positions
          url: /opportunities
      show_form: false
    design:
      css_class: "bg-gradient-to-b from-gray-50 to-white dark:from-gray-900 dark:to-gray-800"
      spacing:
        padding: ["5rem", 0, "5rem", 0]

  - block: cta-card
    content:
      title: Join the RCL Group
      text: We have openings for PhD students, research assistants, visiting graduate students, and postdocs. Please check the positions page for details.
      button:
        text: View Open Positions
        url: /opportunities
    design:
      card:
        css_class: 'bg-primary-300 dark:bg-primary-700'
        css_style: ''
---
