# Numerical Adventures in Geochemical Cycles: A Python Modernization

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

This repository is a modern computational adaptation of the foundational text **"Numerical Adventures with Geochemical Cycles"** by **James C. G. Walker (1991)**. 

While the original book utilized earlier computing paradigms (such as BASIC and manual numerical recipes), this project refactors those lessons into **Python 3** and **Jupyter Notebooks**. It is designed as a self-study course for MSc and PhD students in Earth Sciences, Geochemistry, and Climatology who wish to learn basics of Earth system modeling.

---

## Why Modernize Walker?

James Walker’s approach to geochemical box modeling remains one of the most intuitive ways to understand the feedback loops regulating our planet. However, Walker's "adventures" are still relevant today. This modernization provides:

1.  **Readability:** Python’s syntax allows the geochemistry and climatology to stay at the forefront, rather than the boilerplate code.
2.  **Interactivity:** Jupyter Notebooks allow students to perturb fluxes (e.g., inject a CO2 pulse) and see the system response instantly.
3.  **Modern Toolkits:** Towards the end, we move beyond loops to utilize modern libraries like `NumPy` and `SciPy`.

---

## Course Structure

The repository follows the chapter-by-chapter progression of the original book, with modern enhancements:

### 1. Introduction: Why simulate? (The modern twist)
We discuss simulation not just as a tool for solving equations, but as a  laboratory for "What If" scenarios in the Anthropocene. We also discuss some of the huge computing paradigms that has changed since the original book was published in 1991.

### 2. Chapters 02–08: The adventures
A systematic reconstruction of Walker's box models (his adventures):
* **Mass balance & steady state:** Understanding reservoirs and residence times.
* **The Carbon cycle:** Modeling the thermostat that keeps Earth habitable or over-heating
* **Atmosphere/ocean evolution:** Simulating exchange of species and how it affects climate

### 3. Chapter 09: Numerical Evolution (Euler and Newton-Raphson vs. SciPy)
This chapter provides a brief bridge to modern modeling tools. We compare:
* **The "Old School":** Manual implementation of Euler’s and Newton-Raphson methods as used in the original text.
* **The "Modern Standard":** Utilizing `scipy.integrate.solve_ivp` with adaptive step-size solvers (e.g., RK45 and BDF).
* **The Verdict:** Visualizing numerical drift and understanding why "stiff" geochemical systems require modern algorithms. However, the transparency of Walker's simple solvers might be lost.

---

## Getting started

### Prerequisites
You will need a standard scientific Python environment:
* **Python 3.8+**
* **NumPy** (Numerical arrays)
* **SciPy** (Integration and ODE solvers)
* **Matplotlib** (Visualization)
* **Jupyter/JupyterLab**

### Installation
```bash
# Clone the repository
git clone [https://github.com/olafredin/numerical-adventures-geochemisty-cycles.git](https://github.com/olafredin/numerical-adventures-geochemisty-cycles.git)

# Navigate to the directory
cd numerical-adventures-geochemisty-cycles

# Launch the notebooks
jupyter notebook