# Data Analysis over the OULAD Dataset

![Dataset](https://img.shields.io/badge/dataset-OULAD-blue)

Brief exploratory data analysis and modelling experiments using the Open University Learning Analytics Dataset (OULAD).

**Project Goal:** Analyze student interaction and performance within the OULAD dataset, create clear visualizations, and build baseline models to predict student outcomes.

**Dataset (download):**

- OULAD (Open University Learning Analytics Dataset) — direct download (ZIP):
  https://archive.ics.uci.edu/ml/machine-learning-databases/00349/OULAD.zip

You can download the dataset directly with a command-line tool or your browser. Example (Windows `cmd.exe`):

```bat
curl -L -o OULAD.zip "https://archive.ics.uci.edu/ml/machine-learning-databases/00349/OULAD.zip"
```

If `curl` is not available, use your browser or PowerShell:

```powershell
Invoke-WebRequest -Uri "https://archive.ics.uci.edu/ml/machine-learning-databases/00349/OULAD.zip" -OutFile OULAD.zip
```

After downloading, extract the ZIP (Windows built-in extractor or `tar`):

```bat
tar -xf OULAD.zip
```

Contents
- `diabetes/` — diabetes notebook and CSVs (existing project files)
- `Procastination/` — procrastination notebook (existing project files)
- `Notebooks/` — (recommended) place to put OULAD analysis notebooks

Getting Started

1. Create and activate a Python environment (recommended):

```bat
python -m venv .venv
.venv\Scripts\activate
pip install --upgrade pip
```

2. Install typical data science packages (adjust as needed):

```bat
pip install numpy pandas matplotlib seaborn scikit-learn jupyterlab
```

3. Open Jupyter and start exploring the OULAD data:

```bat
jupyter lab
```

Suggested Notebooks and Analysis
- Exploratory Data Analysis: data cleaning, missing values, distributions, correlations
- Feature Engineering: session-level aggregates, interaction counts, time-based features
- Predictive Models: baseline classifiers (LogisticRegression, RandomForest) to predict pass/fail
- Fairness & Interpretability: feature importance, SHAP or permutation importance

Citation / Source
- The OULAD dataset is maintained by The Open University and hosted on the UCI Machine Learning Repository.

UCI link: https://archive.ics.uci.edu/ml/datasets/Open+University+Learning+Analytics+Dataset

License
- Check the original dataset license from the UCI page before redistribution. This project code is provided under the repository license in `LICENSE`.

Contact
- Author: Ayush — repository: `Ml-Works`
- If you want, I can also add: `requirements.txt`, a sample notebook `Notebooks/OULAD_EDA.ipynb`, or a small data loader script.

Enjoy exploring OULAD — let me know if you want me to scaffold notebooks or add reproducible scripts!
