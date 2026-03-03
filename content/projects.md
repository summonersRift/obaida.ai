---
title: "Projects"
layout: "page"
url: "/projects/"
summary: "Selected projects across AWS Aurora leadership and research systems engineering."
---

Selected projects highlighting technical leadership, system complexity, and end-to-end execution.

## Aurora / AWS (Newer Projects)

### Aurora PostgreSQL Availability Program (MAZ SLA)
**Role:** Engineering leader and execution driver
Raised reliability outcomes for Multi-AZ Aurora PostgreSQL by defining and delivering engine-level capabilities on critical availability paths. Led roadmap, design choices, implementation sequencing, and production readiness to continuously improve SLA outcomes.

### Database Startup and Restart Optimization
**Role:** Technical lead
Led startup and restart-path improvements to reduce downtime during recovery and operational events. Decomposed startup flow into component-level bottlenecks, prioritized high-impact optimizations, and delivered features that improved restart predictability and customer experience.

### Orchestrated Aurora PostgreSQL Upgrades (Ultra-Low Downtime)
**Role:** Upgrade experience lead
Delivered orchestration capabilities for low-downtime engine upgrades while preserving most active database connections. Drove architecture and rollout strategy to balance safety, compatibility, and operational simplicity at production scale.

### Aurora PostgreSQL Serverless v2 Engine Leadership
**Role:** Tech lead
Led core engine initiatives for Aurora PostgreSQL Serverless v2, focusing on elasticity, availability, and long-term architecture direction. Coordinated execution across teams in ambiguous problem spaces while maintaining delivery momentum.

### Aurora Debuggability and Operability Improvements
**Role:** Senior and lead engineer
Improved debuggability and operational signal quality in Aurora PostgreSQL, enabling faster issue isolation and higher-confidence production decision-making.

## Research and Systems Projects (Older Projects)

### Parallel Application Performance Prediction Using Analysis-Based Models and HPC Simulations (PADS 2018, PyPassT)
Designed and implemented PyPassT, an analysis-driven HPC performance modeling framework that converts C/OpenACC applications into executable performance models. The pipeline statically analyzes application structure, captures CPU and GPU work, memory-access behavior, and MPI communication, and executes the model on simulated HPC architectures for rapid what-if analysis. This connected OpenACC code to GPU kernel behavior using NVIDIA CUDA/PTX-informed modeling abstractions and achieved good runtime prediction fidelity on benchmark workloads.

### Simulation of HPC Job Scheduling and Large-Scale Parallel Workloads (WSC 2017)
Built a simulator for evaluating job scheduling algorithms on large HPC systems using PPT (a Python parallel discrete-event simulation framework). By coupling application models with detailed architecture models, the simulator represented realistic runtime behavior and improved evaluation of scheduling and task mapping strategies.

### Integrated Interconnection Network Model for Large-Scale Performance Prediction (PADS 2016)
Contributed to a detailed interconnect model for Cray Gemini 3D torus networks and integrated it with MPI behavior at packet-level fidelity on target platforms. The model improved network behavior prediction accuracy while preserving strong parallel scaling for large simulations.

### On Improving Parallel Real-Time Network Simulation for Hybrid SDN Experimentation (SIMUTOOLS 2017)
Improved parallel real-time network simulation for hybrid simulated/emulated/real experiments by reducing synchronization and distributed communication overheads, enabling better scalability and more practical SDN experimentation workflows.

### Performance Prediction Toolkit (PPT) (2015-2018)
**GitHub:** https://github.com/lanl/PPT
Extended and applied PPT for large-scale performance prediction of applications and architectures, including interconnect, compute, and memory subsystems, to accelerate system design exploration before physical deployment.

### PrimoGENI Constellation (2013-2015)
**GitHub:** https://github.com/netsym/primogeni
Developed distributed, at-scale hybrid network experimentation workflows on GENI resources.
