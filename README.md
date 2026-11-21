# Cognitive Performance Dashboard

An interactive Streamlit and Plotly dashboard for exploring 80,000 records on cognitive performance and lifestyle, and for comparing 11 machine-learning models without writing code.

Built for INDENG 142A (UC Berkeley, Spring 2025), a six-person course project. I built this dashboard.

## What it does

Five tabs:

- **Overview:** summary statistics and the distribution of cognitive levels
- **Regression:** predict cognitive score with linear regression, random forest, a neural network or SVR
- **Classification:** predict cognitive level with random forest, SVM, logistic regression or a neural network
- **Clustering:** k-means, hierarchical clustering or a Gaussian mixture
- **EDA:** distribution, grouped and scatter plots for any feature

Each model has sliders for its main hyperparameters, so a user can change a setting and see the effect at once.

## Data

The Human Cognitive Performance Analysis dataset from Kaggle (80,000 rows, 13 columns). It is not included in this repository. Download it from Kaggle and save it as `human_cognitive_performance.csv` next to `streamlit_app.py`.

## Running it

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

## Limitations

Models are fit on the fly inside the app with simple train/test splits, so the dashboard is for exploring the data and comparing model families, not for final model selection.
