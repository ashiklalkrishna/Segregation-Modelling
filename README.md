# Physics of Social Systems: Modelling the Emergence of Social Divisions

This repository contains a set of **NetLogo models** and a **presentation** developed for the talk **"Physics of Social Systems: Modelling the Emergence of Social Divisions"**, presented at the DysCo Colloquium, Department of Mechanical and Aerospace Engineering, IIT Hyderabad on 04 Oct 2025.

---

## Overview

This work explores how **collective social patterns** can emerge from **simple individual preferences**, inspired by **Schelling’s Segregation Model (1971)**. Through the lens of **complex systems** and **socio-physics**, the models show how local interactions and tolerance thresholds can spontaneously lead to large-scale segregation, even when no individual intends it.

---

## Model Description

Each agent occupies a patch on a 2D grid and belongs to one of two groups (colors).  
Agents evaluate their local neighborhood and decide whether to stay or move based on a **tolerance threshold**.

**Governing Rules**
1. Check neighboring agents.  
2. If the fraction of similar neighbors < threshold → move to a random empty patch.  
3. Repeat until all agents are happy or the system stabilizes.

## Observations

- Over repeated updates, small local moves produce large-scale segregation patterns. 
- Even mild individual preferences can produce strong segregation.  
- The system evolves toward **metastable states**, not perfect equilibrium.  
- Around certain tolerance values, segregation exhibits **critical behavior**, reminiscent of **symmetry breaking** in physical systems.

---

## Repository Contents

| File | Description |
|------|--------------|
| `1_Segregation_relative-density.nlogo` | Basic Schelling's Segregation Model exploring how varying overall and group-wise agent densities influence emergent segregation patterns. |
| `2_Segregation_unhappy-stability.nlogo` | Stops the simulation once the fraction of unhappy agents falls below a specified threshold, instead of waiting for zero unhappiness.|
| `3_Segregation_discrete-threshold.nlogo` | Introduces separate tolerance thresholds for red and blue agents, allowing asymmetric preferences between the two groups. |
| `4_Segregation_relative-similarity-wanted.nlogo` | Explores segregation under a **relative similarity threshold**, allowing heterogeneous perception of neighborhood composition. |
| `5_Segregation_morans-index.nlogo` | Extends the model by computing **Moran’s I**, a spatial autocorrelation measure, to quantify the degree of clustering and spatial segregation between groups. |
| `Dysco Colloquium_Physics of Social Systems.pdf` | Slides presented at the **DysCo Colloquium**|


### How to Run

1. Install [NetLogo](https://ccl.northwestern.edu/netlogo/).  
2. Open any `.nlogo` file in this repository.  
3. Click **Setup** → **Go**.  
4. Adjust parameters such as `%-similar-wanted` and `density` to explore different regimes.

---

## References

**Core References**

- Schelling, T. C. (1971). *Dynamic models of segregation.* Journal of Mathematical Sociology, 1(2), 143–186.  
  [https://doi.org/10.1080/0022250X.1971.9989794](https://doi.org/10.1080/0022250X.1971.9989794)

- Wilensky, U. (1999). *NetLogo.* Center for Connected Learning and Computer-Based Modeling, Northwestern University, Evanston, IL.  
  [https://ccl.northwestern.edu/netlogo/](https://ccl.northwestern.edu/netlogo/)

**Additional Reading**

- Epstein, J. M., & Axtell, R. (1996). *Growing Artificial Societies: Social Science from the Bottom Up.* Brookings Institution Press.  
- Axtell, R. (2001). *Effects of interaction topology and activation regime in several multi-agent systems.* In *Proceedings of the National Academy of Sciences* Workshop on Agent-Based Modeling.  
- Castellano, C., Fortunato, S., & Loreto, V. (2009). *Statistical physics of social dynamics.* Reviews of Modern Physics, 81(2), 591–646.  

---

## Author

**Ashik Lal Krishna**  
Junior Research Fellow
Dynamics and Control Lab
Department of Mechanical and Aerospace Engineering  
Indian Institute of Technology, Hyderabad

---

## Citation

If you reference or adapt this work, please cite as:

> Ashik Lal Krishna. *Physics of Social Systems: Modelling the Emergence of Social Divisions.*  
> DysCo Colloquium, Department of Mechanical and Aerospace Engineering, IIT Hyderabad (2025).

---
