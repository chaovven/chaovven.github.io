---
layout: page
title: "Auto-bidding in E-commerce Advertising"
description: ""
img: /assets/img/publication_preview/wsdm2022_maab.png
importance: 1
category: research
related_publications: false
published: true
---

This project was done during my Internship at Alibaba in 2021, where I collaborated with [Dr. Zhenzhe Zheng](https://zhengzhenzhe220.github.io/) from Shanghai Jiao Tong University and [Zhilin Zhang](https://scholar.google.com/citations?user=ehwxPtEAAAAJ&hl) from Alibaba Group.


## TL;DR

In this project, we developed an RL-driven bidding framework that automates advertiser bids at Internet scale, balancing individual ROI, marketplace welfare, and platform revenue.

<div class="text-center">
  <img src="/assets/img/publication_preview/wsdm2022_maab.png" width="400" />
  <div class="caption">An Overview of the Auto-bidding Services</div>
</div>


## Background

The Auto-bidding in E-commerce Advertising project tackles the fundamental challenge of empowering advertisers on large‐scale online marketplaces to automate their bid decisions under complex, rapidly evolving auction dynamics. In modern e-commerce platforms, billions of ad impressions are auctioned every day across a multitude of campaign objectives—clicks, conversions, add-to-carts—while advertisers operate under strict budget limits and compete both against one another and against the platform’s own revenue goals. The goal of this project is to develop a suite of bidding systems that not only optimize each advertiser’s return on investment, but also maintain a healthy, high-welfare marketplace and robust platform revenues.


## Key Takeaways

In this project, we proposed a cooperative-competitive multi-agent bidding framework for auto-bidding in online advertising, MAAB, which jointly optimizes advertiser utility, social welfare, and platform revenue. The key takeaways are:

- Online advertising auctions are mixed cooperative-competitive multi-agent systems, requiring a nuanced approach to balance individual advertiser utility, collective social welfare, and platform revenue.
- Revenue degradation, a common issue in cooperative multi-agent reinforcement learning, can be effectively mitigated using adversarial training with "bar agents" without altering the underlying auction mechanism.
- Scaling multi-agent reinforcement learning to millions of agents in industrial settings is feasible by employing a mean-field approach, grouping agents by objective and inferring individual actions from group-level policies.


## Key Results

- Offline simulations on Alibaba's industrial dataset showed that our proposed MAAB framework achieved superior social welfare compared to competitive baselines and significantly higher revenue than cooperative baselines, striking an optimal balance.
- Online A/B tests on Alibaba's real production environment showed our proposed MAAB framework increased social welfare by 4.6% compared to a competitive multi-agent baseline, with a 3.9% decrease in revenue.
- Ablation studies confirmed that Temperature-Regularized Credit Assignment (TRCA) effectively balances cooperative and competitive behaviors, and personalized bar agents are crucial for preventing revenue loss.


## Links

- Paper: [https://doi.org/10.1145/3488560.3498373](https://doi.org/10.1145/3488560.3498373)
- Code: [https://github.com/chaovven/maab](https://github.com/chaovven/maab)