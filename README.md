# The AIT Physicist: Quantifying the Algorithmic Information Dynamics of Financial Crises

**Authors:** Yeu Wen Mak

**Repository for:** *The Computational Phase Transition: Detecting Financial Crises via Algorithmic Information Dynamics*

---

## 1. Abstract & Core Contribution
This repository contains the codebase, datasets, and reproducible notebooks for the **AIT Physicist**, a transformer-based diagnostic tool for financial time series. 

Building upon the statistical "Coherence Meter" framework, this work replaces the first-order proxy (predictive error) with a second-order inference engine (Algorithmic Information Theory). By mapping financial data to the **Wolfram Computational Universe** (Elementary Cellular Automata), we demonstrate that financial crises are not merely volatility events, but distinct **Computational Phase Transitions**.

**Key Findings:**
1.  **Early Warning:** A systematic validation on the CrunchDAO dataset (N=200) reveals a mean detection lead time of **-27.07%** relative to official structural breaks.
2.  **Taxonomy of Crashes:** We identify two distinct topological signatures of market collapse:
    *   **Systemic Decay (2008):** Preceded by **Class 4 Saturation** (Rule 54/Solitons).
    *   **Exogenous Shock (2020):** Characterized by **Class 3 Chaos** (Rule 60/Fractals).

---

## 2. The Repository Structure

*   **`ait_lib/`**: The core Python library containing:
    *   `model.py`: The Tiny Recursive Model (TRM) architecture.
    *   `pipelines.py`: Quantile encoding and Entropy calculations.
    *   `train.py`: Logic for pre-training the Physicist on ECA rules.
*   **`notebooks/`**:
    *   `01_The_Training_Ground.ipynb`: Pre-training the Transformer on the 256 ECA rules.
    *   `02_The_Gauntlet.ipynb`: Systematic validation on CrunchDAO Structural Break data (Source of the -27% statistic).
    *   `03_The_Showdown.ipynb`: Historical analysis of 2008, 2018, and 2020 (Source of the Phase Portraits).
*   **`data/`**: (Instructions on where to place CrunchDAO parquet files).
*   **`results/`**: CSV exports of detection logs and rule frequency distributions.

---

## 3. Reproducibility
To replicate the findings of the paper:

1.  **Provision the Physicist:** Run `notebooks/01_The_Training_Ground.ipynb` to generate `trm_expert.pth`.
2.  **Validate Statistics:** Run `notebooks/02_The_Gauntlet.ipynb` to reproduce the Lag Distribution Histogram.
3.  **Visualize History:** Run `notebooks/03_The_Showdown.ipynb` to generate the 2008/2020 Phase Portraits.

---

## 4. Theoretical Background
This work integrates three distinct fields:
*   **Algorithmic Information Theory (AIT):** Treating markets as computational systems (Zenil, Delahaye).
*   **SuperARC Framework:** Defining intelligence/coherence as algorithmic compression (Hernández-Espinosa et al.).
*   **Econophysics:** Mapping market regimes to Wolfram Complexity Classes.

---
