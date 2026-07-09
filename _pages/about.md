---
layout: about
title: about
permalink: /
subtitle:

profile:
  align: right
  image: prof_pic.png
  image_circular: true # crops the image to make it circular
  more_info: >
    

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am an Operations Research scientist interested in optimization systems for scarce resource allocation under uncertainty. My work sits between mathematical optimization, production decision systems, and infrastructure-scale resource allocation.

## Background

My interest in allocation problems started during my master’s thesis at [École Polytechnique de Montréal](https://www.polymtl.ca/), where I worked on the classic vertex coloring problem under the guidance of [Alain Hertz](https://www.gerad.ca/~alainh/) and [Martine Bellaïche](https://www.polymtl.ca/expertises/en/bellaiche-martine). Later, I spent close to a decade, in the workforce management industry, architecting and building forecasting and large-scale autoscheduling systems for real operational environments. More recently, I worked at Amazon on reinforcement-learning-based inventory replenishment policy optimization.

I am currently completing a Ph.D. in Operations Research at [Cornell University](https://www.duffield.cornell.edu/orie/), advised by [Brenda Dietrich](https://www.duffield.cornell.edu/people/brenda-lynn-dietrich/) and [Jamol Pender](https://www.duffield.cornell.edu/people/jamol-j-pender/). My research focuses on Mixed Integer Programming (MIP) solvers performance variability.

## Interests

- Resource allocation
- Large-scale scheduling & Capacity planning
- Forecasting 
- Simulation-based policy evaluation
- Stochastic and robust optimization
- Reliable Mathematical programming systems


---

## Featured Project

### Compute Capacity Orchestrator  
**[Simulation-optimization for GPU workload scheduling and AI infrastructure performance modeling](/projects/)**  

Compute Capacity Orchestrator is a public research-engineering project for studying how scarce GPU capacity should be allocated when jobs arrive over time, wait in queues, compete for limited accelerator resources, and require scheduling decisions within practical latency budgets.

The current release includes greedy and exact snapshot schedulers, closed-loop simulation, decision validation, operational metrics, regression tests, and a Streamlit dashboard.

The roadmap extends the system toward topology-aware GPU orchestration, including solver latency budgets, capacity fragmentation, GPU locality, NVLink and InfiniBand/Ethernet fabric effects, rolling-horizon scheduling, stochastic demand scenarios, and scale-up versus scale-out placement tradeoffs.

The project combines ideas from mathematical programming, discrete-event simulation, and production systems design.



