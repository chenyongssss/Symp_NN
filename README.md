```markdown
# Symplectic ROM — Numerical Experiments

This repository hosts three numerical experiment suites:
- `linear/` — 1D linear wave
- `param/`  — parametric linear wave
- `schro/`  — 1D nonlinear Schrödinger (NLS)

Each folder contains two Jupyter notebooks:
1) **Data generation** (run first)
2) **Model building / training / testing** (run second)

## Repository layout
```

.
├── linear/
├── param/
└── schro/

````

## Environment
- Python ≥ 3.10
- JupyterLab/Notebook
- NumPy, SciPy, Matplotlib, Pandas
- TensorFlow ≥ 2.12 (or the version used in your paper)

Quick setup (example):
```bash
conda create -n symprom python=3.11 -y
conda activate symprom
pip install numpy scipy matplotlib pandas jupyterlab tensorflow
````

## How to run (same for all examples)

Using `linear/` as an example:

1. Open `linear/linear_data_generation.ipynb` and **Run All**.
   This writes `data/features.npy` (and 'labels.npy', optional 'test.npy').
2. Open `linear/symp_linear_wave.ipynb` and **Run All**.
   

> The `param/` and `schro/` folders follow the same procedure.

## Reproducibility

Each notebook sets random seeds at the top. Keep defaults or change them explicitly.

## Data size

If full datasets are large, commit a small sample for quick reproduction and provide a generator/downloader inside the data notebook. If you use Git LFS, configure `.gitattributes` accordingly.

## Issues

Please include your OS, Python/TensorFlow versions, and a screenshot of any error when filing an issue.

````