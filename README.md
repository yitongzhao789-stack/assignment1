# Zomato Data Science Assignment

This project performs feature engineering, regression & classification modeling, and evaluation on the Zomato dataset. Git, DVC, and Git LFS are used for full pipeline reproducibility.

---

## Installation

```bash
# Option 1: Using conda
conda create -n zomato-assign python=3.11 -y
conda activate zomato-assign
conda install -c conda-forge pandas numpy scikit-learn matplotlib seaborn plotly kaleido geopandas folium pyproj shapely pyspark dvc joblib pyyaml -y

## How to Run the Project

# This project uses DVC for reproducible pipelines. Follow the steps below:
# 1. Clone the repo and enter the directory
git clone https://github.com/Yitongzhao789-stack/assignment1.git
cd assignment1

# 2. Pull large data/model files with Git LFS
git lfs pull

# 3. Reproduce the full pipeline
dvc repro

# Expected Results
Cleaned dataset stored at: outputs/clean/clean.csv
Trained model file at: outputs/model/model.pkl
Visualizations stored in: outputs/figures/*.png
Final notebook: U3287758_assignment1.ipynb contains metrics comparison and analysis

