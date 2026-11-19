# Results

| Folder | Produced by | Files |
|---|---|---|
| `02_phase1_optuna_random_split/` | notebooks `02_*` | `Optuna_Results_MLO.csv`, `Optuna_Results_BRW.csv` |
| `03_chronological_raw/` | notebook `03_*` (MLO; BRW by setting `LOCATION='BRW'`) | `Optuna_Results_MLO.csv` |
| `04_phase2_dt_sq_optuna/` | notebooks `04_*` | `Optuna_Sequential_Results_MLO.csv`, `Optuna_Sequential_Results_BRW.csv` |

The Phase 1 Bayesian baseline notebooks (`01_*`) print their metrics in the notebook output and do not write a CSV.

Metrics are computed on the held-out test set in ppm (MSE, RMSE, MAE in ppm; MAPE in percent; R2 dimensionless).

Note on provenance: the files in `02_*` and `04_*` were transcribed from the result tables printed in the saved notebook outputs (the corresponding CSVs written by the original Colab runs were overwritten). Re-running a notebook regenerates the CSV in the same folder; stochastic LSTM training can change the deep-learning rows in the last digits.
