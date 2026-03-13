# MATD3-UAV-Disaster-Search

This repository contains the implementation and evaluation code for the paper:

**Dynamic Task Allocation and Path Planning for Multi-UAV Disaster Search Using Multi-Agent Reinforcement Learning**

## Overview

This project proposes a multi-agent reinforcement learning framework for cooperative UAV inspection in disaster-response environments.
The approach is based on **Multi-Agent Twin Delayed Deep Deterministic Policy Gradient (MATD3)** with centralized critics under the CTDE (Centralized Training with Decentralized Execution) paradigm.

The framework enables multiple UAVs to autonomously coordinate their motion and task assignments while avoiding collisions and efficiently reaching inspection targets.

Two inspection scenarios are considered:

* **Roof inspection:** UAVs inspect the rooftop of damaged structures.
* **Mid-height inspection:** UAVs inspect intermediate sections of buildings, enabling multiple UAVs to inspect different parts of the same structure.

The proposed approach is compared against baseline methods including a simplified baseline policy and the **TANet-TD3** framework.

---

## Repository Structure

```
MATD3-UAV-Disaster-Search-Code
│
├── Baseline comparison
│   ├── Our baseline
│   └── TANET paper baseline
│
├── Proposed Algorithms
│   ├── Midheight_inspection
│   └── Roof_inspection
│
├── Demo videos
│
└── README.md
```

### Baseline comparison

Contains training and evaluation logs for baseline approaches used in the paper, including:

* Simplified baseline implementation
* TANet-TD3 baseline results
* Evaluation metrics and logs at each folder

### Proposed Algorithms

Contains the implementation of the proposed **MATD3-based UAV coordination framework**.

Two experiment configurations are included:

* **Midheight_inspection:** UAVs inspect mid-level building targets.
* **Roof_inspection:** UAVs inspect rooftop targets.

Each folder contains:

* training scripts / notebooks
* trained models
* evaluation logs
* experiment outputs

### Demo videos

Demonstration videos showing the UAV behavior in the simulated disaster environment.

---

## Evaluation Metrics

The experiments evaluate the system using:

* Task success rate
* Episode length (mission completion time)
* Collision counts between UAVs and obstacles

The proposed MATD3 framework demonstrates improved coordination efficiency and reduced collision rates compared with the baseline approaches.

---

## Requirements

Typical dependencies include:

* Python 3.x
* PyTorch
* NumPy
* Matplotlib
* Jupyter Notebook

---

## Reproducing Experiments

Experiments can be reproduced by running the training or evaluation scripts inside each scenario folder:

```
Proposed Algorithms/Midheight_inspection
Proposed Algorithms/Roof_inspection
```

The provided logs and trained models allow direct evaluation of the policies reported in the paper.

---

## Demo

Example videos demonstrating UAV coordination and inspection behavior are available in the **Demo videos** directory.

---

## Citation

If you use this code in your research, please cite the corresponding paper.

---

## Contact

Malek Chabbouh
computer engineering, Qatar University
chmalek2@gmail.com
