
[![QAMP Project](https://img.shields.io/badge/QAMP-2025-blue)](https://qiskit.org/advocates)  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)  [![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)  [![GPAW](https://img.shields.io/badge/GPAW-TDDFT-green)](https://wiki.fysik.dtu.dk/gpaw/)  [![Qiskit](https://img.shields.io/badge/Qiskit-Quantum%20ML-purple)](https://qiskit.org/)

## Q-UCSpec: Integrating TDDFT Spectroscopy and Quantum Machine Learning for Photonic Upconversion Materials

**Q-UCSpec** is a QAMP 2025 project that integrates **first-principles Linear Response (Lr) Time-Dependent Density Functional Theory (TDDFT)** simulations with **Quantum Machine Learning (QML)** to explore the optical spectra of **photonic upconversion materials**.  

The project focuses on:
- Generating TDDFT absorption spectra for host and doped systems (CaF₂ + Ca₃F:Er clusters).  
- Extracting spectral descriptors (first moment, variance, peak energy, spectral area).  
- Encoding these features into quantum feature maps with Qiskit.  
- Benchmarking QSVM / EstimatorQNN against classical ML models.

This project is part of the **Qiskit Advocate Mentorship Program (QAMP) 2025**.  

---

### Repository Structure

```bash
Q-UCSpec/
├── simulations/        # ASE + GPAW scripts for CaF2, Ca3F:Er clusters
├── spectra/            # TDDFT stick and broadened spectra (CSV)
├── features/           # Extracted spectral descriptors for ML/QML
├── qiskit/             # Quantum ML notebooks (QSVM, EstimatorQNN)
├── docs/               # Documentation and project notes
└── README.md
```

---
### ⚙️ Installation & Setup
```python
# Clone Repo
git clone https://github.com/denniswayo/Q-UCSpec.git
cd Q-UCSpec

# Create conda environment
conda create -n q-ucspec python=3.9
conda activate q-ucspec

# Install dependencies
conda install -c conda-forge gpaw ase scipy matplotlib
pip install qiskit qiskit-machine-learning

# Test installation
python -c "import gpaw; import ase; import qiskit; print('YES! Environment ready')"
```
---

### Mentorship
Mentor: Dennis Wayo (@DennisWayo)
QAMP 2025 Project: Q-UCSpec

```bash
Mentees will:
	•	Learn lr-TDDFT workflow with GPAW + ASE.
	•	Run simulations of photonic upconversion clusters.
	•	Apply QML with Qiskit to spectral datasets.
	•	Contribute code, documentation, and benchmarking analysis.
[DavidAlba2627](https://github.com/DavidAlba2627)  [keremyurtseven](https://github.com/keremyurtseven)  [Siriapps](https://github.com/Siriapps)  [Alireza1988](https://github.com/Alireza1988)  [GHOST-Q1](https://github.com/GHOST-Q1)  [DreamzUpAbove](https://github.com/DreamzUpAbove)
```

### Acknowledgements
	•	Qiskit Advocate Mentorship Program (QAMP) @qiskit-advocate @IBM
	•	ASE + GPAW developers @gpaw @ase
	•	Qiskit Machine Learning team
	•	Research inspiration: Photonic upconversion in CaF₂:Er system
