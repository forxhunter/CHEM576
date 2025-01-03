## **Week 8: Whole Cell Kinetic Modeling and Simulations**

* TOC
  {:toc}

### **1. Overview of Whole-Cell Modeling**

Whole-cell modeling aims to simulate every process occurring inside a cell, including:

* **Gene Expression** : Transcription and translation of genes into proteins.
* **Metabolism** : Conversion of nutrients into energy and biomass.
* **Coupling Mechanisms** : Interactions between gene expression, metabolic fluxes, and cellular growth.

---

### **2. Reaction-Diffusion Master Equation (RDME)**

* **Purpose** : Models biochemical reactions in a spatially resolved system.
* **Key Concepts** :
* **Stochastic Reactions** : Random reaction events occur based on reaction propensities.
* **Diffusion** : Molecules diffuse between compartments, influencing spatial gradients.

---

### **3. Lattice Microbes (LM)**

 **URL** : [https://www.ks.uiuc.edu/Research/lm]()

* **Purpose** : A GPU-accelerated software package for simulating stochastic reaction-diffusion systems.
* **Key Features** :
* Simulates RDME for large-scale cellular processes.
* Optimized for parallel computation on GPUs.
* Tracks molecular trajectories and reactions over time.
* **Tutorial** : Official tutorials available at [Lattice Microbes Documentation]().
