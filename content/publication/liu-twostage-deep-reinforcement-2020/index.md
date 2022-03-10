---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Two-Stage Deep Reinforcement Learning for Inverter-Based Volt-VAR Control in
  Active Distribution Networks
subtitle: ''
summary: ''
authors:
- admin
- Wenchuan Wu
tags:
- '"deep reinforcement learning"'
- '"Games"'
- '"Markov processes"'
- '"Reactive power"'
- '"reactive power."'
- '"Reinforcement learning"'
- '"Safety"'
- '"Training"'
- '"transfer learning"'
- '"Voltage control"'
categories: ['Featured work']
date: '2020-01-01'
lastmod: 2021-02-27T23:35:41+08:00
featured: false
draft: false
weight: 100

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
publishDate: '2021-02-27T15:38:40.760398Z'
publication_types:
- '2'
abstract: Model-based Vol/VAR optimization method is widely used to eliminate voltage
  violations and reduce network losses. However, the parameters of active distribution
  networks(ADNs) are not onsite identified, so significant errors may be involved
  in the model and make the model-based method infeasible. To cope with this critical
  issue, we propose a novel two-stage deep reinforcement learning (DRL) method to
  improve the voltage profile by regulating inverter-based energy resources, which
  consists of offline stage and online stage. In the offline stage, a highly efficient
  adversarial reinforcement learning algorithm is developed to train an offline agent
  robust to the model mismatch. In the sequential online stage, we transfer the offline
  agent safely as the online agent to perform continuous learning and controlling
  online with significantly improved safety and efficiency. Numerical simulations
  on IEEE test networks not only demonstrate that the proposed adversarial reinforcement
  learning algorithm outperforms the state-of-art algorithm, but also show that our
  proposed two-stage method achieves much better performance than the existing DRL
  based methods in the online application.
publication: '*IEEE Transactions on Smart Grid*'
doi: 10.1109/TSG.2020.3041620
---
