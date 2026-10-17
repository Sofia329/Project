# Data Science Portfolio — Airbnb, Time‑Series Forecasting & AdaBoost 

> Disclaimer these Projects are for USYD Master of Quant Finance & Big Data coursework

This repository contains three data‑science projects demonstrating end‑to‑end workflows in exploratory analysis, feature engineering, modeling, and evaluation. The projects are suitable for a GitHub portfolio and showcase both applied machine learning and time‑series forecasting skills, plus a from‑scratch ensemble algorithm implementation.

---

## Projects Overview

1. **Airbnb Price Prediction (Airbnb Project.ipynb)**
   - Goal: Predict nightly listing price using Airbnb listing features from Sydney.
   - Highlights: extensive EDA, text and categorical feature engineering, model comparison (linear models, tree ensembles, boosting), and final predictive model with validation strategy.
   - Useful for: hosts, investors, and pricing strategy analysis.

2. **Time Series Forecasting — Unemployment Rate (Time Series Data Prediction.ipynb)**
   - Goal: Forecast monthly unemployment rates using historical series.
   - Highlights: time‑series decomposition, trend/seasonality analysis, SARIMA and neural approaches, and model comparison (MSE/RMSE metrics).
   - Useful for: macroeconomic analysis, policy planning, and forecasting practice.

3. **AdaBoost Classifier (AdaBoost.py)** - Goal: Educational implementation of AdaBoost using decision stumps as weak learners.
   - Highlights: demonstrates boosting loop, adaptive sample weighting, alpha calculation, and ensemble voting. Includes an option to use logistic regression as a base learner.
   - Useful for: learning ensemble internals and custom estimator development.

---

## Repository Structure

- `Airbnb Project.ipynb` — notebook with the Airbnb analysis and predictive modeling pipeline.
- `Time Series Data Prediction.ipynb` — notebook with time‑series exploration and forecasting experiments.
- `AdaBoost.py` — custom AdaBoost classifier implementation (script / module).
- `requirements.txt` — Python dependencies for running the notebooks and scripts.
- `README.md` — this file.

> Note: raw data files are not included in the repository. Add a `data/` folder and the original dataset CSVs when reproducing the analyses.

---

## Quickstart — Run locally

1. Clone the repository:

```bash
git clone https://github.com/Sofia329/Project.git
cd Project
```

2. (Optional) Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate   # macOS / Linux
venv\Scripts\activate    # Windows (PowerShell)
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run the notebooks:

```bash
jupyter lab   # or `jupyter notebook`
# then open the two notebooks:
# - "Airbnb Project.ipynb"
# - "Time Series Data Prediction.ipynb"
```

5. Run the AdaBoost script (example; you will need to provide a dataset or unit tests):

```bash
python AdaBoost.py
```

---

## Reproducibility & Tips

- Add a `data/` directory and place original CSV files there (or update notebook paths). Notebooks currently expect CSVs in the working directory.
- If a notebook uses GPU‑accelerated models (Keras/TensorFlow), ensure the correct TensorFlow package is installed and configured.
- To reproduce exact results, pin dependency versions in `requirements.txt` (provided in this repo) and run in a clean virtual environment.

---

## Results & Next Steps

- Add a `results/` folder with figures, model artifacts and a short `report.md` summarizing key findings (MAE/RMSE, feature importance, pros/cons of models).
- Move large datasets outside the repo (or add them to a release), and keep notebooks focused on code + reproducible analysis.
- Consider converting long notebooks into modular scripts under a `src/` folder for production‑ready workflows.

---

## License & Contact

This repository is provided for educational and portfolio purposes. If you plan to reuse data or code outside personal study, check the original dataset licenses and attribute sources accordingly.

If you have questions or want help improving structure, tests, or CI, open an issue or contact: **Sofia329** on GitHub.
