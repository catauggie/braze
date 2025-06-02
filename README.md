# Optimal Thermal Trajectory Planning for Induction Brazing

This repository contains code and supporting material for the research articles:

**Automated Induction Brazing Control System Based on Optimal Trajectory Planning** &

**Dual-loop proportional control for high-precision inductionbrazing of thin-walled aluminum waveguides**

---

## Overview

The goal of this work is to optimize the spatial and temporal characteristics of induction heat sources in automated brazing systems. The optimization targets thermal trajectories that closely match a desired reference profile while minimizing energy waste and signal oscillations.

Three main objectives are considered:
1. **Accuracy** — match the target temperature profile.
2. **Symmetry** — minimize the difference between reference and symmetric source configurations.
3. **Smoothness** — suppress high-frequency fluctuations via derivative control.
4. https://disk.yandex.ru/d/1hE-ljyEwSSvXA - program module

Multi-objective optimization is performed using the NSGA-II algorithm from [pymoo](https://pymoo.org). The results are visualized through Pareto fronts and thermal response curves.

---

## Contents

| File                | Description                                                   |
|---------------------|----------------------------------------------------------------|
| `Braze optimal.ipynb` | Main Jupyter Notebook for simulation and optimization (Python + pymoo). |
| `one_obj.pdf`        | Plot of the temperature profile for single-objective optimization.         |
| `single_obj.pdf`     | Visualization of results from scalarized optimization setup.              |
| `tri_obj.pdf`        | Pareto front projection for the three-objective optimization case.        |

---

## Reproducibility

### Dependencies
- Python 3.9+
- `numpy`, `matplotlib`
- `pymoo` (for multi-objective optimization)

Install all dependencies using:
```bash
pip install numpy matplotlib pymoo
