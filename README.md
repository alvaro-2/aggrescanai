# AggrescanAI  
**Prediction of Aggregation Prone Regions (APRs) in proteins using contextual embeddings.**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/alvaro-2/aggrescanai/blob/main/aggrescanai.ipynb) 🡄 To launch AggrescanAI press this button.  

<p align="center">
    <img src="docs/aggrescanai_logo.png" alt="AggrescanAI logo" width="300">
</p>  


## Overview
Protein aggregation plays a dual role in biology and biotechnology. On one hand, it is a **central mechanism in neurodegenerative diseases** such as Alzheimer’s, Parkinson’s and ALS; on the other, it represents a **major bottleneck in protein engineering**, affecting solubility, stability and yield.  
APR identification is therefore key for both **understanding disease mechanisms** and **optimizing protein design**.  

**AggrescanAI** is a deep learning–based tool for residue-level prediction of aggregation-prone regions (APRs) directly from protein sequences.  
It leverages **contextualized embeddings** from the **ProtT5 protein language model**, capturing biochemical and structural information implicitly encoded in sequence data — without requiring 3D structural input.  

---


## Key Features

- Predicts **residue-level aggregation propensity** directly from sequence.  
- **No structural data required**, applicable to folded and disordered proteins.  
- Employs **ProtT5 embeddings (1024-dimensional)** to capture sequence context.   
- **Homology-augmented datasets** to enhance generalization.  
- **Validated against experimental benchmarks**.  
- Detects **aggregation shifts caused by pathogenic mutations**.  
- Fully open and **accessible via Google Colab**, no installation required.

---


## Methodology

### Workflow Summary

1. **Input**: A protein sequence.  
2. **Embedding generation**: Each residue is encoded as a 1024-dimensional vector using *ProtT5 pretrained model*.  
3. **Prediction**: A deep neural network processes each residue embedding.  
4. **Output**: Residue-level aggregation propensity profile.  


---

## Usage

You can run AggrescanAI directly from Google Colab through an interactive notebook interface — no installation required.

### Steps

1. **Open the Colab notebook:**  
   👉 [Launch AggrescanAI in Google Colab](https://colab.research.google.com/github/alvaro-2/aggrescanai/blob/main/aggrescanai.ipynb)

2. **Set up your input:**  
   In the **form-like section** at the top of the notebook, you can:
   - Enter a **UniProt ID** (e.g. `P10636-8`)  
   - *or* paste a **protein sequence** directly.  
   - Optionally tick **“use_example”** to load a demo sequence.

3. **Run all cells** by selecting *Runtime → Run all* or pressing `Ctrl+F9`.

4. **Visualize and download results:**  
   The notebook will display a **residue-level aggregation profile** (table + figure) and allow you to download the output files.

---

## How to cite this work?

If you use AggrescanAI in your research, please cite:

[![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.jmb.2026.169643-blue)](https://doi.org/10.1016/j.jmb.2026.169643)

**Navarro, A. M., Palacios, S., Galmarini, T., Bárcenas, O., Ventura, S., & Marino-Buslje, C.** (2026). AggrescanAI: Prediction of Aggregation-Prone Regions Using Contextualized Embeddings. *Journal of molecular biology*, 169643. https://doi.org/10.1016/j.jmb.2026.169643

---
