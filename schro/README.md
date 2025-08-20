```markdown
# Example: 1D Nonlinear Schrödinger (NLS)

This example demonstrates data generation and training/evaluation for the 1D NLS problem.

## Files
- `schro_data_generation.ipynb` — generate/preprocess data (initial condition, periodic BCs, step sizes)  
  **Outputs:** `data/features.npy` ('labels.npy')
- `symp_schrodinger.ipynb` — build/train the model and evaluate (includes Hamiltonian-related plots)  
  **Outputs:** `runs/<timestamp>/` (logs, checkpoints, figures)

## Run order
1. Run `schro_data_generation.ipynb`.
2. Run `symp_schrodinger.ipynb`.
```


## Notes
- If you observe numerical instability, reduce the time step or switch to a more stable discretization (see comments in the data notebook).
- Enable the Hamiltonian monitoring callbacks/metrics in the training notebook if needed.
