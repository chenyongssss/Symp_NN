```markdown
# Example: Parametric Linear Wave

This example handles **parametric** linear waves (e.g., varying speed/coefficients).

## Files
- `param_data_generation.ipynb` — generate parametric datasets (parameter ranges, sampling strategy)  
  This writes `data/features.npy` (and 'labels.npy', optional 'test.npy'). with parameter metadata.
- `symp_param.ipynb` — build/train the model and test 
  **Outputs:** `runs/<timestamp>/` (logs, checkpoints, figures)

## Run order
1. Run `param_data_generation.ipynb`.
2. Run `symp_param.ipynb`.



## Notes
- If train/test parameter distributions differ, record the details in `data_generation.ipynb`.
- For quick tests, reduce the number of parameter samples.
```