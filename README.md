# Reconciling Metabolic Networks and Population-Level Models
**A Hybrid FBA-ODE-Stochastic Framework**

This repository contains the Python implementation of a multi-scale computational framework that bridges the gap between intracellular metabolic constraints and ecological population dynamics.

By coupling **Flux Balance Analysis (FBA)** with **Stochastic Chemical Reaction Networks (CRN)** and **Ordinary Differential Equations (ODEs)**, this model demonstrates how microscopic noise in gene expression creates emergent macroscopic phenomena—specifically, the metabolic "lag phase" observed when bacteria adapt to complex carbon sources like Maltose.

## 🚀 Key Features

* **Hybrid Modeling:** Integrates deterministic metabolic solvers (COBRApy) with stochastic gene regulation (MobSpy).
* **Dynamic Coupling:** Metabolic uptake bounds ($v_{max}$) are dynamically updated based on the real-time accumulation of transporter enzymes.
* **Emergent Lag Phases:** Successfully reproduces biological lag phases for Maltose vs. Glucose without using empirical Monod parameters.
* **Quantized Growth:** Captures "staircase" growth dynamics driven by single-molecule events.

## 📦 Prerequisites

You need **Python 3.8+** and the following scientific libraries:

* **COBRApy:** For metabolic constraint-based modeling.
* **MobSpy:** For stochastic simulation (Gillespie algorithm) of gene networks.
* **NumPy:** For numerical operations.
* **Matplotlib:** For data visualization.

### Installation

Install all dependencies via pip:

```bash
pip install numpy matplotlib mobspy cobra
```

## 🏃‍♂️ How to Run

There are two ways to run the simulation:

### Option 1: Jupyter Notebook (Recommended)
1. Launch Jupyter Lab or Notebook:
   ```bash
   jupyter notebook
   ```

   