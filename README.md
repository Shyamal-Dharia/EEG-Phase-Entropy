# EEG-Phase-Entropy

Official implementation for the paper:

**Dual-Transformer Cross-Attention Framework for Alzheimer’s disease detection via dPTE-Guided EEG channel selection and multi-modal integration**

---

## Graphical Abstract

<p align="center">
  <img src="figures/GA.png" alt="Graphical Abstract" width="600">
</p>

---

## Overview

This repository provides the full set of codes used for DTCA-Net, a dual-transformer cross-attention architecture that integrates:

- **directed Phase Transfer Entropy (dPTE)** for connectivity-driven channel selection  
- **Differential Entropy (DE)** for spectral complexity  
- **Cross-attention fusion** aligning connectivity (queries) and spectral features (keys/values)

DTCA-Net achieves high performance for Alzheimer’s disease (AD) and Frontotemporal Dementia (FTD) detection while using only **six EEG channels** identified by dPTE: F7, F8, T3, T4, O1, O2.

---

## Repository Structure

    EEG-Phase-Entropy/
    │
    ├── figures/
    │ ├── GA.png
    │ └── model_diagram.png
    │
    ├── src/
    │ ├── feature_extraction.ipynb
    │ ├── PTE_calculation_final.ipynb
    │ ├── DE_Transformer.ipynb
    │ ├── PTE_Transformer.ipynb
    │ └── Dual_Input_Transformer.ipynb
    │
    ├── README.md
    └── requirements.txt


---

## Installation

```bash
git clone https://github.com/<your-user>/EEG-Phase-Entropy.git
cd EEG-Phase-Entropy

python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

pip install -r requirements.txt

```

## Citation

    @article{DHARIA2026108390,
      title   = {Dual-Transformer Cross-Attention Framework for Alzheimer’s disease detection via dPTE-Guided EEG channel selection and multi-modal integration},
      author  = {Shyamal Y. Dharia and Qian Liu and Stephen D. Smith and Camilo E. Valderrama},
      journal = {Biomedical Signal Processing and Control},
      volume  = {112},
      pages   = {108390},
      year    = {2026},
      doi     = {10.1016/j.bspc.2025.108390}
    }


