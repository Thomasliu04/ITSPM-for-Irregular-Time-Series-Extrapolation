# ITSPM for Irregular Time Series Extrapolation

HKUST ARIN6900 Independent Project — ITSPM Task 1.3.

This project studies irregular multivariate time series forecasting
using the provided ITSPM framework.

This task focuses on IMTS extrapolation, which forecasts the future values of each variable at given query timestamps from irregular historical observations. The student will reproduce ITSPM on benchmarks such as PhysioNet 2012, Human Activity, and USHCN following the standard t-PatchGNN-style protocol. ITSPM will be compared with lightweight forecasting baselines. The analysis centers on the soft temporal kernel branch and on how multi-scale continuous-time patterns help at different forecast horizons.
- Milestone 1 – Reproduce the main results. Train ITSPM on two or three datasets with the default observation and forecast windows. Report MSE/MAE over three seeds and compare them with the provided reference results.
- Milestone 2 – Lightweight baselines. Evaluate naive baselines (last-value persistence and per-variable linear extrapolation), and train lightweight neural baselines such as GRU-D and mTAND. Report all results in a unified table and comment on the gap between naive and learned forecasters.
- Milestone 3 – Temporal kernel ablation and sensitivity analysis. Remove the soft temporal kernel branch, and vary the number of temporal scales and the kernel bandwidths to study their effects. Analyze sensitivity to history length and forecast horizon, and plot error versus horizon for ITSPM and the baselines.
- Milestone 4 – Visualization and analysis. Visualize forecasts alongside the observed history for selected samples, and plot the learned temporal kernels (e.g., kernel shapes and weights across scales). Discuss how kernel scale relates to dataset characteristics such as sampling rate and periodicity, and analyze typical failure cases.
