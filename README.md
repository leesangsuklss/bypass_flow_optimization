# Multi-Objective Optimization for novel RO vessel design

This repository contains a Python implementation for analyzing and optimizing **Seawater Reverse Osmosis (SWRO)** processes. The framework focuses on the introduction of new bypass flow feature and performs multi-objective optimization to find optimal bypass flow rates and locations to balance system performance metrics.

## Key Features

* **Thermophysical Property Modeling**: Implements correlations for seawater *density*, *viscosity*, and *osmotic pressure* as a function of temperature and salinity.
* **Numerical modeling of full-scale RO pressure vessels**: Models the impact of different conditions on the system performances.
* **Multi-Objective Optimization**: optimized for competing objectives using `pymoo.optimize`.
* **Visualization**: Includes tools for analyzing trade-offs (Pareto frontiers).

---

## Scientific Background
The code is based on thermodynamic models for full-scale RO system. Key correlations used in this work include:

Density & Viscosity: Sharqawy et al. correlations for seawater.

Osmotic Pressure: Pitzer equations or simplified correlations for NaCl solutions.

Membrane Transport: Solution-Diffusion model with Arrhenius temperature dependence.

Note: The optimization logic with the pymoo library considers the trade-off between energy consumption (kWh/m³) and irreversible losses.

---

**Launch the Notebook directly**  
    ```
    jupyter notebook MV_OPT_multi-objective_SW_conc_wrapper.ipynb
    ```
