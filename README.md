# mini-project-kaggle-disaster-tweets

**Project:** Kaggle-style mini project for classifying disaster-related tweets.

**Overview**
- **Purpose:** Explore, preprocess, and model the Kaggle "Disaster Tweets" dataset to predict whether a tweet describes a real disaster (target = 1) or not (target = 0).
- **Primary artifact:** `disaster_tweets_nlp.ipynb` — a notebook with EDA, preprocessing, modelling experiments, and inference examples.

**Data (in `data/`)**
- **`train.csv`**: labeled training set (commonly: `id`, `text`, `location`, `target`).
- **`test.csv`**: unlabeled test set for final inference.
- **`sample_submission.csv`**: example submission format for Kaggle.
- **`submission.csv` / `submission_enhanced.csv`**: example or local submission files created during experimentation.

**Quick Start**
1. Create and activate a Python virtual environment (PowerShell):

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

2. Install dependencies (utilize the `requirements.txt`):

   ```powershell
   pip install -r requirements.txt
   ```

3. Start Jupyter and open the notebook:

   ```powershell
   jupyter lab   # or jupyter notebook
   ```

4. Open `disaster_tweets_nlp.ipynb` and run cells top-to-bottom.

**Notebook Contents**
- **Exploratory Data Analysis (EDA):** class balance, common words, locations, and tweet lengths.
- **Preprocessing:** cleaning, tokenization, stopword handling, optional lemmatization/stemming.
- **Feature engineering:** bag-of-words, TF-IDF, simple embeddings, or transformer encodings.
- **Modeling:** baseline classifiers (Logistic Regression, Random Forest), simple pipelines, and optional transformer-based approaches.
- **Evaluation & Submission:** cross-validation, validation metrics (accuracy, F1), and saving a `submission.csv` following `sample_submission.csv` format.

**Reproducibility Notes**
- If you add heavy models (transformers / GPU), pin package versions in `requirements.txt` and document hardware used.
- Random seeds: set seeds for NumPy, Python, and model libraries inside the notebook to make results reproducible.

**Suggested Next Steps**
- Add a `requirements.txt` or `environment.yml` for reproducible installs.
- Create scripts to run training and inference outside the notebook (e.g., `train.py`, `predict.py`).
- Add unit tests for preprocessing functions and a lightweight CI workflow.

**Contributing**
- Fork the repo, create a feature branch, and open a pull request describing your changes.
- For big experiments, add a short README or notebook summarizing new approaches and results.

**License & Contact**
- No license specified. If you want to reuse this code, please contact the repository owner: `dyegofern` on GitHub.

If you'd like, I can also:
- generate a `requirements.txt` from the notebook imports,
- extract and create small runnable scripts (`train.py`, `predict.py`), or
- run a quick environment check to list missing packages.
# mini-project-kaggle-disaster-tweets