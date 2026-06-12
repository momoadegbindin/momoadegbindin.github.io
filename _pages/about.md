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

I build optimization systems for messy real-world decisions: who works when, where inventory should sit, how scarce resources should be allocated, and why mathematical programming solvers sometimes fail when production needs them most.
I care about optimization systems that are mathematically sound, highly explainable, and reliably useful to the people who depend on them. 

## Academic Training

### Ph.D., Operations Research | Cornell University
My Ph.D. in Operations Research focuses on MIP solver performance variability: rare runtime tails, timeouts, and branch-and-bound trajectory changes on difficult instances. I have worked with SCIP internals in C++ and large-scale computational studies.

### M.A.Sc., Computer Engineering | École Polytechnique de Montréal
Prior to my doctoral track, I earned my Master's degree in Computer Engineering and my thesis focused on designing a greedy algorithm to the classic Vertex Coloring Problem (VCP).

### Industrial Experience
Before graduate school, I spent close to a decade building production optimization systems for workforce management, scheduling, forecasting, and resource allocation (Kronos/Workbrain). The main system I worked on was a configurable MIP-based autoscheduler used across roughly 40 customer deployments and millions of scheduled employees/users. It replaced customer-specific scheduling logic with a reusable optimization engine and reduced schedule generation from days of manual planning to minutes.

Recently at Amazon, I scoped and built an end-to-end reinforcement learning framework for inventory replenishment policy optimization, with projected savings opportunities in the hundreds of millions if generalized at scale.


---
## Selected Projects

### Scarce Compute Allocation Sandbox
A production-style optimization framework for GPU workload scheduling, queueing, and cluster capacity policy evaluation. This repository simulates cluster environments to test and benchmark mathematical scheduling policies under resource constraints.

#### [Topology-Aware GPU Cluster Batch Scheduler](/projects/)
An optimization module within the sandbox that minimizes cross-node network synchronization latency during large-scale distributed training runs. The engine maps parallel workloads onto multi-tier cluster fabrics by solving the underlying assignment problems.
*   **Techniques:** Mixed-Integer Linear Programming (MILP), Benders Decomposition, Column Generation, Stochastic/Robust Optimization with recourse, Metaheuristics, and Discrete-Event Simulation.
*   **Stack:** Python (Pyomo, SciPy), automated verification via `pytest`.
*   **Status:** *In Active Development.* Currently implementing the multi-period recourse matrices and hardware topology networks.




