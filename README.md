# Multi-Objective Optimization for SWRO Concentration

This repository contains a Python implementation for analyzing and optimizing **Seawater Reverse Osmosis (SWRO)** processes. The framework focuses on the **temperature dependence** of seawater thermophysical properties and performs **multi-objective optimization** to balance system performance metrics.

## Key Features

* **Thermophysical Property Modeling**: Implements correlations for seawater *density*, *viscosity*, and *osmotic pressure* as a function of temperature and salinity.
* **Temperature Dependence Analysis**: Models the impact of feed water temperature on RO membrane transport parameters ($A$ and $B$ values).
* **Multi-Objective Optimization**: optimized for competing objectives (e.g., **Minimizing SEC** vs. **Maximizing Concentration**) using `scipy.optimize`.
* **Visualization**: Includes tools for analyzing trade-offs (Pareto frontiers) using `seaborn` and `matplotlib`.

---

## Scientific Background
The code is based on thermodynamic models for electrolyte solutions. Key correlations used in this work include:

Density & Viscosity: Sharqawy et al. correlations for seawater.

Osmotic Pressure: Pitzer equations or simplified correlations for NaCl solutions.

Membrane Transport: Solution-Diffusion model with Arrhenius temperature dependence.

Note: The optimization logic considers the trade-off between energy consumption (kWh/m³) and irreversible losses.
