# anisopol

Efficient protein polarization-energy estimation using a compact model of **anisotropic atomic polarizabilities** and **bond-resolved electric-field descriptors**.

This repository contains:
- Code to **compute and decompose local electric fields** from background point charges;
- Code to **fit direction-dependent atomic polarizability parameters** against QM reference polarization energies (example: **ALA** fitting set);
- Code to **predict polarization energies for peptides/proteins** under explicit-solvent electrostatic embedding (example: **PDB 1L2Y** test set).

---

## Code & Data Availability

- GitHub (code): https://github.com/Renws/anisopol  
- Zenodo (example datasets): https://zenodo.org/records/18256166

The Zenodo archive provides example data for:
- **ALA fitting dataset** (training/parameter optimization)
- **1L2Y test dataset** (protein polarization-energy evaluation)

---

## Installation

### Recommended environment
Python 3.9+ is recommended.

```bash
git clone https://github.com/Renws/anisopol.git
cd anisopol

# creat conda environment
conda create -n anisopol python=3.10 -y
conda activate anisopol

# Install dependencies
pip install numpy os tqdm json time
