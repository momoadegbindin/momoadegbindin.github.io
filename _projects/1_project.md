---
layout: page
title: Scarce Compute Allocation Sandbox
description: optimization and simulation for compute-capacity decisions
img: assets/img/DataCenter.jpg
importance: 1
category: work
related_publications: false
---

A research sandbox for studying compute-capacity allocation under uncertainty.

The project will model workloads, queues, cluster capacity, and scheduling policies in a controlled simulation environment. The goal is to compare simple heuristics, optimization-based policies, and bounded-time decision rules under congestion and capacity shocks.

**Methods:** mathematical programming, scheduling heuristics, queueing, and discrete-event simulation.  
**Status:** in active development.  
**Repository:** [GitHub](https://github.com/momoadegbindin/)

## Initial design

```text
workloads → queue → scheduler → cluster state → metrics
