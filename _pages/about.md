---
layout: about
title: about
permalink: /
subtitle:

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Ithaca, NY</p>

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

My interest in allocation problems started during my master’s thesis at [École Polytechnique de Montréal](https://www.polymtl.ca/), where I worked on the classic vertex coloring problem under the guidance of [Alain Hertz](https://www.gerad.ca/~alainh/) and [Martine Bellaiche](https://www.polymtl.ca/expertises/en/bellaiche-martine). It became much more practical later in the workforce management industry, where I spent close to a decade architecting and building forecasting and large-scale autoscheduling systems for real operational environments. More recently, I worked at Amazon on reinforcement-learning-based inventory replenishment policy optimization.

I am currently completing a Ph.D. in Operations Research at [Cornell University](https://www.duffield.cornell.edu/orie/), advised by [Brenda Dietrich](https://www.duffield.cornell.edu/people/brenda-lynn-dietrich/) and [Jamol Pender](https://www.duffield.cornell.edu/people/jamol-j-pender/). My research focuses on Mixed Integer Programming (MIP) solvers performance variability.

## Interests

- Large-scale scheduling
- Resource allocation
- Capacity planning
- Simulation-based policy evaluation
- Mathematical programming systems that remain reliable under production constraints


---
## Selected Projects

### Scarce Compute Allocation Sandbox
A production-style optimization framework for GPU workload scheduling, queueing, and cluster capacity policy evaluation. This repository simulates cluster environments to test and benchmark mathematical scheduling policies under resource constraints.

#### [Topology-Aware GPU Cluster Batch Scheduler](/projects/)
An optimization module within the sandbox that minimizes cross-node network synchronization latency during large-scale distributed training runs. The engine maps parallel workloads onto multi-tier cluster fabrics by solving the underlying assignment problems.
*   **Techniques:** Mixed-Integer Linear Programming (MILP), Benders Decomposition, Column Generation, Stochastic/Robust Optimization with recourse, Metaheuristics, and Discrete-Event Simulation.
*   **Stack:** Python (Pyomo, SciPy), automated verification via `pytest`.
*   **Status:** *In Active Development.* Currently implementing the multi-period recourse matrices and hardware topology networks.




