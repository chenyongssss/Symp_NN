```markdown
# Example: Linear Wave

This example covers data generation and training/evaluation for the 1D linear wave problem.

## Files
- `linear_data_generation.ipynb` — generate/preprocess train/test data  
  This writes `data/features.npy` (and 'labels.npy', optional 'test.npy').
- `symp_linear_wave.ipynb` — build the model, train, and evaluate  
  **Outputs:** `runs/<timestamp>/` (logs, checkpoints, figures)

## Run order
1. Run `linear_data_generation.ipynb` first and verify files appear under `data/`.
2. Run `symp_linear_wave.ipynb` to train and evaluate.
```


## Notes
- Start with a smaller grid or shorter time horizon to smoke-test the pipeline, then scale up.
- If training time is long, reduce `epochs`, `batch_size`, or model width/depth.
