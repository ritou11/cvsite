---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Online Multi-Agent Reinforcement Learning for Decentralized Inverter-Based
  Volt-VAR Control
subtitle: ''
summary: ''
authors:
- admin
- Wenchuan Wu
tags: []
categories: ['Featured work']
date: '2021-01-01'
lastmod: 2021-02-27T23:36:40+08:00
featured: true
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2021-02-27T15:28:40.498463Z'
publication_types:
- '2'
abstract: The distributed Volt/Var control (VVC) methods have been widely studied
  for active distribution networks(ADNs), which is based on perfect model and real-time
  P2P communication. However, the model is always incomplete with significant parameter
  errors and such P2P communication system is hard to maintain. In this paper, we
  propose an online multi-agent reinforcement learning and decentralized control framework
  (OLDC) for VVC. In this framework, the VVC problem is formulated as a constrained
  Markov game and we propose a novel multi-agent constrained soft actor-critic (MACSAC)
  reinforcement learning algorithm. MACSAC is used to train the control agents online,
  so the accurate ADN model is no longer needed. Then, the trained agents can realize
  decentralized optimization using local measurements without real-time P2P communication.
  The OLDC with MACSAC has shown extraordinary flexibility, efficiency and robustness
  to various computing and communication conditions. Numerical simulations on IEEE
  test cases not only demonstrate that the proposed MACSAC outperforms the state-of-art
  learning algorithms, but also support the superiority of our OLDC framework in the
  online application.
publication: '*IEEE Transactions on Smart Grid*'
doi: 10.1109/TSG.2021.3060027
---
