---
layout: page
title: Scarce Compute Allocation Sandbox
description: optimization and simulation for compute-capacity decisions
img: assets/img/12.jpg
importance: 1
category: work
related_publications: false
---

A research sandbox for studying how scarce compute capacity can be allocated under congestion, uncertainty, and operational constraints.

The project treats compute allocation as a production decision problem: workloads arrive over time, capacity is limited, service targets matter, and scheduling policies must balance utilization, reliability, and delay.

[GitHub repository](https://github.com/YOUR-USERNAME/YOUR-REPO)

## Overview

The sandbox is designed to compare scheduling and capacity policies in a controlled environment. It models a simplified compute cluster where workloads compete for limited resources under queueing, deadlines, runtime uncertainty, and capacity shocks.

The goal is not to reproduce any real cloud system. The goal is to build a clean experimental environment for asking practical questions:

- When does a simple greedy policy fail?
- How much value does optimization add under congestion?
- What happens when demand spikes or capacity drops?
- How should a bounded-time scheduler behave when exact optimization is too slow?
- Which policies improve utilization without damaging reliability?

## Architecture

The first version is organized around four layers:

- **Workload generator** — creates synthetic jobs with resource needs, priorities, deadlines, and runtime uncertainty.
- **Cluster model** — represents limited compute capacity, queue state, and operational constraints.
- **Scheduling policies** — compares greedy, exact, and hybrid bounded-time scheduling approaches.
- **Simulation and evaluation** — tests policies over time under congestion, failures, and changing demand.

## Methods

The project combines ideas from:

- mathematical programming;
- scheduling heuristics;
- discrete-event simulation;
- queueing models;
- policy evaluation for production systems.

## Status

In active development.

The initial implementation focuses on a small but complete version: workload generation, baseline scheduling policies, simulation, metrics, and reproducible experiments. More advanced extensions will be added only after the core system is working and tested.
