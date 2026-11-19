# DPA – Online Retail Data Analysis

M.Tech CSE (Artificial Intelligence), 2026  
Subject: Data Preparation and Analysis

## Project overview
This project analyzes the Online Retail transaction dataset using Python, NumPy, Pandas, Matplotlib, Seaborn, Plotly and scikit-learn. It covers data collection, NumPy operations, Pandas inspection, cleaning, EDA, static and interactive visualizations, feature engineering, conclusions and GitHub submission guidance.

## Dataset
- Kaggle: https://www.kaggle.com/datasets/vijayuv/onlineretail
- Original UCI documentation: https://archive.ics.uci.edu/dataset/352/online+retail

Download `OnlineRetail.csv` and place it in the same folder as the notebook. The notebook also checks `/content/OnlineRetail.csv` for Google Colab.

## Files
- `DPA_Online_Retail_Analysis.ipynb` – completed analysis notebook
- `requirements.txt` – Python dependencies

## Run locally
```bash
python -m pip install -r requirements.txt
jupyter notebook DPA_Online_Retail_Analysis.ipynb
```
Run all cells from top to bottom.

## Data cleaning notes
Exact duplicates are removed; invoice dates are parsed; missing descriptions are filled as `Unknown`; missing customer IDs are retained as missing; zero-quantity and non-positive-price records are excluded. Negative quantities are retained because they can represent returns. Outliers are identified using IQR and are not automatically deleted.

## Important
Check the dataset's licence and terms before uploading the CSV itself to a public GitHub repository.
