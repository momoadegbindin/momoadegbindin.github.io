---
layout: page
title: Compute Capacity Orchestrator
description: Optimization and simulation for GPU workload scheduling
img: assets/img/Compute_Capacity_Orchestrator.png
importance: 1
category: work
related_publications: false
---

<img src="/assets/img/Compute_Capacity_Orchestrator.png" alt="Compute Capacity Orchestrator hero" width="100%">

Compute Capacity Orchestrator (CCO) is a simulation-optimization framework for GPU workload scheduling, compute-capacity allocation, and AI infrastructure performance modeling.

The project studies a central infrastructure question: when accelerator capacity is scarce, how should jobs be queued, prioritized, placed, and dispatched so that expensive GPU resources stay productive without creating backlog, deadline risk, fragmentation, or excessive scheduler latency?

CCO models synthetic workloads, waiting queues, limited GPU capacity, scheduling policies, validation, state transitions, and operational metrics in one controlled environment. The current public release supports greedy scheduling, exact snapshot optimization with Pyomo/HiGHS, closed-loop simulation, and a Streamlit dashboard for inspecting policy behavior.

The longer-term direction is topology-aware and rolling-horizon GPU orchestration: modeling GPU types, NVLink locality, InfiniBand/Ethernet fabric effects, solver latency budgets, scale-up versus scale-out placement tradeoffs, stochastic demand scenarios, and hybrid bounded-time scheduling.

## Why This Project Matters

Modern AI infrastructure is not only a hardware problem. It is a resource-allocation problem under uncertainty.

Poor scheduling can leave expensive accelerators idle, strand capacity across fragmented nodes, delay high-priority work, or spend too much time searching for an optimal schedule that arrives too late to be operationally useful.

CCO makes those tradeoffs measurable. It compares scheduling decisions using metrics such as GPU utilization, queue length, wait time, deadline risk, value captured, and runtime per decision.

## Current Implementation

The current release includes:

- Typed schemas for jobs, resources, topology, scheduling snapshots, assignments, and decisions
- Synthetic workload and cluster scenario generation
- Greedy snapshot scheduling
- Exact snapshot MIP scheduling using Pyomo/HiGHS
- Decision validation against snapshot feasibility
- Closed-loop simulation with arrivals, waiting jobs, running jobs, completed jobs, and GPU release
- Metrics for utilization, queue length, wait time, deadline risk, objective value, and scheduler runtime
- Streamlit dashboard with snapshot and simulation views
- Regression tests across schemas, engines, validation, metrics, scenarios, simulation, and dashboard data builders

## System Design

The project is organized around four layers:

1. **Workload and cluster modeling**  
   Generates GPU jobs with demand, priority, release time, duration, and deadline information, then represents limited accelerator capacity at the node level.

2. **Scheduling engines**  
   Implements interchangeable scheduling policies, including fast greedy rules and an exact snapshot MIP. Future engines will include rolling-horizon and hybrid bounded-time policies.

3. **Simulation and state transition**  
   Evolves the queue and cluster over time by admitting new jobs, invoking the scheduler, applying validated decisions, completing jobs, and releasing GPUs.

4. **Metrics and dashboard**  
   Reports operational behavior through utilization, backlog, wait time, deadline risk, value captured, and scheduler runtime.

## Technical Direction

Planned extensions include:

- Time-indexed MIP formulations over a short planning horizon
- Rolling-horizon scheduling for anticipatory capacity allocation
- Hybrid bounded-time scheduling with fallback behavior
- Topology-aware placement with GPU types, NVLink locality, rack structure, and InfiniBand/Ethernet fabric effects
- Capacity-fragmentation metrics
- Stochastic demand scenarios and capacity shocks
- Decomposition-based solver experiments for larger planning and placement models

## Methods

Mathematical programming, scheduling heuristics, simulation optimization, queueing systems, stochastic and robust optimization, policy evaluation, and AI infrastructure performance modeling.

## Repository

[GitHub](https://github.com/momoadegbindin/compute-capacity-orchestrator)


