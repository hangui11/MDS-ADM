# Project: NEURAL OBLIVIOUS DECISION ENSEMBLES FOR DEEP LEARNING ON TABULAR DATA

## Contents
- `methods_comparison.ipynb`: Main Jupyter notebook for running experiments.
- `requirements.txt`: List of required Python packages.
- `data/wdbc/wdbc.data`: The dataset used for experiments.
- `data/wdbc/wdbc.names`: Dataset description and attribute information.

## Step-by-Step Instructions

### 1. Install Python
- **Required Version:** Python 3.8 or higher (recommended: Python 3.9 or 3.10)
- **Download:** https://www.python.org/downloads/
- **How to check if Python is installed:**
  - Open Terminal (Mac) or Command Prompt (Windows)
  - Type: `python --version` or `python3 --version`

### 2. Install pip (Python package manager)
- **Usually comes with Python.**
- **Check if installed:**
  - Type: `pip --version` or `pip3 --version`
- **If not installed, see:** https://pip.pypa.io/en/stable/installation/

### 3. Install Jupyter Notebook
- In your terminal, run:
  - `pip install notebook`

### 4. Install Project Dependencies
- Navigate to the project folder in your terminal. Example:
  - `cd /Users/admin/Desktop/ADM`
- Install all required packages by running:
  - `pip install -r requirements.txt`

### 5. Dataset
- The dataset is already included in the folder: `data/wdbc/wdbc.data`
- Dataset description is in: `data/wdbc/wdbc.names`
- **Source:** [UCI Machine Learning Repository - WDBC](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))

### 6. Run the Notebook
- Start Jupyter Notebook by running:
  - `jupyter notebook`
- In the browser window that opens, click on `methods_comparison.ipynb` to open it.
- Run the cells one by one (Shift+Enter) to execute the code and see results.

## Troubleshooting
- If you get errors about missing packages, try running `pip install <package_name>` for each missing package.
- If you have both `python` and `python3` on your system, you may need to use `python3` and `pip3` instead of `python` and `pip`.

## Required Python Packages (with minimum versions)
- pytorch-tabular
- scikit-learn
- pandas
- numpy
- catboost
- xgboost
- typing-extensions