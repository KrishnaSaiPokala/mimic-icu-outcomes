# Predictive Modeling of ICU Outcomes (MIMIC-IV)

![Status](https://img.shields.io/badge/status-portfolio%20project-blue) ![Python](https://img.shields.io/badge/python-3.x-informational) ![MIMIC-IV](https://img.shields.io/badge/MIMIC-IV-relevant-lightgrey) ![Clinical Prediction](https://img.shields.io/badge/Clinical%20Prediction-relevant-lightgrey) ![SQL](https://img.shields.io/badge/SQL-relevant-lightgrey)

Clinical prediction workflow with cohort definition, validation checks and structured evaluation.

## Why this project matters
This project shows healthcare data judgment, feature construction, leakage prevention and more structured evaluation than a simple model-score-first workflow.

## Project purpose
This repository documents a graduate portfolio project completed in healthcare and biomedical analytics. The goal was to build a workflow that is clear, reviewable and grounded in sound data handling rather than only optimizing for a headline model score.

## Project highlights
- Defined an early-ICU prediction cohort
- Built time-windowed feature tables from vitals, labs, demographics and comorbidity records
- Added validation checks for missingness, duplicates, unit consistency and timestamp alignment
- Reviewed calibration, subgroup behavior and failure patterns

## Dataset
- **Dataset:** MIMIC-IV
- **Task:** Early prediction of in-hospital mortality from ICU data

## Workflow
1. Define the cohort and prediction window
2. Build SQL and Python feature tables
3. Apply validation checks
4. Train baseline and comparison models
5. Evaluate AUROC, PR-AUC, calibration and subgroup behavior

## Methods and tools
- SQL
- Python
- Pandas
- NumPy
- scikit-learn
- Time-windowed feature engineering
- Validation checks
- Leakage prevention
- Calibration review
- Subgroup error analysis

## Results
This project established a structured early-ICU prediction workflow with attention to feature validity, leakage prevention and evaluation beyond a single metric. Calibration review and subgroup checks were useful for understanding where performance was stronger and where limitations remained.

Planned additions to this repository:
- final AUROC and PR-AUC results
- calibration plot
- subgroup performance summary
- brief notes on failure patterns and limitations

## Repository structure
- `notebooks/` project walkthrough and exploratory work
- `src/` preprocessing, training and evaluation scripts
- `outputs/figures/` saved charts, plots or calibration figures
- `outputs/metrics/` summary text or metric tables
- `docs/` short project notes or exported summaries
- `assets/` images used in the README if needed

## How to run
```bash
pip install -r requirements.txt
python src/preprocess.py
python src/train.py
python src/evaluate.py
