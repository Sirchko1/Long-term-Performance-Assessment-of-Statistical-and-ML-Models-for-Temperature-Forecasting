# Long-term Performance Assessment of Statistical and ML Models for Temperature Forecasting

This repository contains the dataset, core models, and statistical validation scripts for the research article: **"Long-term Performance Assessment of Statistical and ML Models for Temperature Forecasting in Coastal Cities of the Gulf of Mexico"** (Currently under review).

## Overview
This project proposes the compare 9 diverse forecasting approaches (Classical, Machine Learning, and Deep Learning) using a static hold-out test set approach againts a hybrid model**FMFRA**, measure with the performance metrics (RMSE, sMAPE, DA) and residual analyses are evaluated across 30 independent executions.

## Repository Structure
* `/data`: Contains the historical temperature datasets for Tampico, Matamoros, Miami, and Houston.
* `/scripts`: Includes the architecture of the proposed FMFRA model and the scripts used for step-by-step empirical optimization.
* `/scripts/statistical_tests`: Python scripts for executing the non-parametric Friedman test, Iman-Davenport correction, and the post-hoc Wilcoxon signed-rank test with Holm-Bonferroni adjustment.
* `/results`: Contains the raw outputs of the 30 independent runs and the matrices used for calculating the Mean Bias Error (MBE).

## Reproducibility
To reproduce the statistical validation presented in the paper:
1. Clone this repository.
2. Install dependencies: `pip install -r requirements.txt`
3. Run the statistical evaluation script: `python scripts/statistical_tests/wilcoxon_tests.py`

## Citation
If you use this code or dataset in your research, please cite our paper:
