# Universal and Lightweight Electricity Load Forecasting Model

This project presents a lightweight, generalizable electricity demand forecasting framework based on LightGBM, designed to perform reliably across cities with diverse consumption patterns. It incorporates minimal but effective temporal features such as `load_lag1` and `load_avg3`, aiming for computational efficiency and cross-city adaptability.

## 📁 Repository Structure

The repository consists of three main zipped folders:

### 🔧 `work.zip`
Contains code scripts and notebooks for training and evaluation:
- `AS2.ipynb`: Main notebook for LightGBM model training and evaluation.
- `AS2 other ML models.ipynb`: Includes comparisons with other machine learning models (e.g., SVM, RF, NN).
- `piecewise.py`, `plot_template.py`, `utlis.py`: Python utilities for modeling, plotting, and evaluation.

### 📊 `data.zip`
Includes preprocessed, hourly electricity load data for five cities:
- `fuzhou_hourly_modified.xlsx`
- `singapore_hourly_modified.xlsx`
- `la_hourly_modified.xlsx`
- `ny_hourly_modified.xlsx`
- `sac_hourly_modified.xlsx`

All datasets contain hourly-level demand and meteorological features.

### 📂 `results.zip`
Stores the output of the models and visualization figures:
- Feature importance tables (`feature_importance_all_cities.csv`)
- Performance visualizations (e.g., heatmaps, seasonal trends, bar plots)
- Model output CSVs (`lgbm_*.csv.csv`)

## 💡 Highlights
- Adaptable across cities with different load patterns
- Lightweight, interpretable features (no deep learning or heavy preprocessing required)
- Strong baseline performance with minimal tuning

## 📌 How to Use
1. Unzip all three folders into your working directory.
2. Open and run `AS2.ipynb` to replicate the main experiments.
3. Use `AS2 other ML models.ipynb` to compare performance across ML models.
4. Visualizations and evaluation outputs can be found in the `/results` folder.

## 🔬 Future Work
- Integration of additional temporal or socioeconomic features
- Automated feature tuning (e.g., Bayesian optimization)
- Testing in more regions beyond the current dataset

---

📫 For questions or collaboration: feel free to open an issue or reach out via email.
