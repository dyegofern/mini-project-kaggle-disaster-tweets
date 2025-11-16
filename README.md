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

# mini-project-kaggle-disaster-tweets