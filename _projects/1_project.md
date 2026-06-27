---
layout: page
title: Compute Capacity Orchestrator
description: Optimization and simulation for GPU workload scheduling
img: assets/img/DataCenter.jpg
importance: 1
category: work
related_publications: false
---

# Compute Capacity Orchestrator

**Optimization and simulation for GPU workload scheduling**

Compute Capacity Orchestrator is a research sandbox for studying GPU workload scheduling and compute-capacity decisions under uncertainty.

The project models synthetic workloads, waiting queues, limited cluster capacity, and scheduling policies in a controlled simulation environment. The goal is to compare fast heuristics, optimization-based policies, and hybrid bounded-time decision rules under congestion, workload-mix changes, and capacity shocks.

The first version focuses on a simple end-to-end pipeline: generate jobs, model available GPU capacity, evolve the queue over time, make scheduling decisions, and report operational metrics.

## Initial Design

The project is organized around four layers:

1. **Workload generator**
   Creates synthetic GPU jobs with resource needs, priorities, release times, duration estimates, deadlines, and runtime uncertainty.

2. **Cluster model**
   Represents limited compute capacity, queue state, GPU availability, and operational constraints.

3. **Scheduling policies**
   Compares greedy, exact, and hybrid bounded-time scheduling approaches.

4. **Simulation and metrics**
   Evaluates policies over time using utilization, queue length, wait time, deadline risk, value captured, scheduler runtime, and fallback behavior.

## Methods

Mathematical programming, scheduling heuristics, queueing simulation, discrete-event simulation, and policy evaluation.

## Status

In active development.

## Repository

GitHub.
[GitHub](https://github.com/momoadegbindin/compute-capacity-orchestrator)


