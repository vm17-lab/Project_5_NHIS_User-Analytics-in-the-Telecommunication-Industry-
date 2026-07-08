# User-Analytics-in-the-Telecommunication-Industry-

## 📋 Overview

Telecom operators generate massive volumes of session-level data every day, but that data is rarely used to its full potential. This project cleans and enriches a real-world telecom dataset, explores user behavior across handsets and applications, and applies **K-Means clustering** to group subscribers into distinct engagement segments — light, moderate, and power users — that map directly onto business decisions like bundle design, network capacity planning, and churn prevention.

## 🎯 Objectives

- Clean and standardize a messy, high-dimensional telecom dataset
- Engineer per-application traffic features (Social Media, Google, Email, YouTube, Netflix, Gaming, Other)
- Explore user behavior through univariate, bivariate, and multivariate analysis
- Identify relationships between handset manufacturer, network throughput, and data consumption
- Determine the optimal number of user segments using the Elbow Method and Silhouette Score
- Build and validate a K-Means clustering model to segment users by engagement
- Translate each cluster into a clear business recommendation

## 🗂️ Repository Structure

```
.
├── Unsupervised telecom data.ipynb   # Main notebook: cleaning, EDA, feature engineering, clustering
├── telecom_sql.ipynb                 # Loads cleaned data into SQL Server (SQLAlchemy / pyodbc)
├── Telecom_Presentation.pptx         # Summary slide deck of findings and recommendations
├── telecom_cleaned_compressed.zip    # Cleaned dataset (compressed CSV)
├── Screenshot 2026-07-07 204111.png  # Reference screenshot (SQL)
├── LICENSE                           # MIT License
└── README.md
```

## 🛠️ Tech Stack

- **Language:** Python
- **Data manipulation:** pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine learning:** scikit-learn (`StandardScaler`, `KMeans`, `PCA`, `silhouette_score`, `train_test_split`)
- **Database:** SQL Server via SQLAlchemy / pyodbc
- **Environment:** Jupyter Notebook

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn sqlalchemy pyodbc
```

### Running the analysis
1. Clone this repository
   ```bash
   git clone https://github.com/vm17-lab/Project_5_NHIS_User-Analytics-in-the-Telecommunication-Industry-.git
   ```
2. Unzip the cleaned dataset
   ```bash
   unzip telecom_cleaned_compressed.zip
   ```
3. Open and run `Unsupervised telecom data.ipynb` in Jupyter to reproduce the cleaning, EDA, and clustering steps.
4. (Optional) Run `telecom_sql.ipynb` to load the cleaned data into a local SQL Server instance.

## 📑 Deliverables

- **Notebook:** `Unsupervised telecom data.ipynb` — full analysis and modeling pipeline
- **Presentation:** `Telecom_Presentation.pptx` — summarized findings for a business audience
- **Cleaned dataset:** `telecom_cleaned_compressed.zip`

## 📄 License

This project is licensed under the [MIT License](LICENSE).
