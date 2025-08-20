```markdown
# Symplectic ROM — Numerical Experiments

This repository contains code for three numerical experiment suites:
- `linear/` — 1D linear wave equation
- `param/` — Parametric linear wave equation
- `schro/` — 1D nonlinear Schrödinger (NLS) equation

Each folder contains two Jupyter notebooks:
1. **`*_data_generation.ipynb`**: Run this first to generate the simulation data.
2. **`symp_*.ipynb`**: Run this second to build, train, and test the symplectic reduced-order model.



## Environment Setup

The code requires:

- Python ≥ 3.10
- JupyterLab or Jupyter Notebook
- NumPy, SciPy, Matplotlib, Pandas
- TensorFlow ≥ 2.12

A quick setup using `conda` is recommended:
```bash
conda create -n symprom python=3.11 -y
conda activate symprom
pip install numpy scipy matplotlib pandas jupyterlab tensorflow
```

## How to Run

The procedure is the same for all examples. Using the `linear/` experiment as an example:

1.  **Generate Data**: Open and run all cells in `linear/linear_data_generation.ipynb`.
    *This will generate `data/features.npy` (and typically `labels.npy`; a `test.npy` may also be created).*
2.  **Train and Test Model**: Open and run all cells in `linear/symp_linear_wave.ipynb`.

> The `param/` and `schro/` folders follow the identical procedure.

## Reproducibility

Each notebook sets random seeds at the beginning for reproducibility. Please keep the default seed values or change them explicitly if needed.

## Data Size

The full datasets used in the paper may be large. This repository includes smaller sample datasets to allow for quick verification and reproduction of the code. Instructions for generating full datasets or links to download them are provided in the respective data generation notebooks.

