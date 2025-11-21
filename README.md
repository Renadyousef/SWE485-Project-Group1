# Spam Advice System and Detection  – SWE485

## Why We Chose This Topic
We chose this project because phishing and spam emails are one of the most common cybersecurity threats today.  
Being able to automatically detect them helps protect users and organizations from scams and data leaks.

---

## Team Members

| Name | Student ID |
|------|------------|
| Fajer Alkatheri        | 443204563 | 
| Renad Alotibi          | 443200801 | 
| Rawan Khaled           | 443204623 | 
| Rahaf Samkari          | 443202844 | 
| Salha Abdullah Shahbal | 443204567 |

---

## Dataset
- Source: [Phishing Email Dataset on Kaggle](https://www.kaggle.com/datasets/naserabdullahalam/phishing-email-dataset)  
- Contains around **39,000 emails** labeled as *Spam (1)* or *Legitimate (0)*.  
- Key columns include:  
  - `subject`, `body`: email text  
  - `urls`, `receiver_spam_ratio`, `capital_ratio`: extracted numeric features  
  - `label`: target variable

---

## What We Did in Phase 1
- Cleaned the dataset and handled missing values.  
- Extracted new useful features from emails.  
- Processed text data and converted it to numerical form using **TF-IDF**.  
- Scaled numeric features and combined them with text vectors.  
- Saved all processed data for the next phase (model training).

---

## What We Did in Phase 2
- Split the data into **train** and **test** sets.  
- Trained **three different models** and evaluated their performance.  
- Chose the best-performing model.  
- Captured high-weight features in text for analysis.  
- Applied error analysis (underfit, overfit, good fit) and removed highly correlated columns (cheating columns).

---

## What We Did in Phase 3 – Unsupervised Clustering
In Phase 3, we performed **K-Means clustering** to analyze the natural structure of the email dataset.  
This phase was **analytical only** — no new supervised models were trained.

**Summary of Phase 3:**
- Applied K-Means clustering with different values of K.  
- Found **optimal clusters (K=4)** using the Silhouette Score (~0.57).  
- Used **PCA** for visualization and to observe cluster separation.  
- Compared clusters to **true labels** to understand how spam and non-spam emails distribute naturally.  
- Observed **internal spam sub-patterns**, which are not explicitly captured by supervised models.

**Key Insights:**
- Emails naturally form **meaningful clusters** based on features.  
- **Spam emails** tend to group together, supporting why supervised models performed well.  
- Phase 3 confirmed that the dataset has **strong internal structure**, even without labels.  
- Clustering is **not required for spam detection**, but it helps **explain model behavior** and reinforces confidence in the supervised approach.

---

## Files in This Repository

- `Phase1_Data_Exploration.ipynb` ← Notebook for data exploration, feature extraction, and TF-IDF transformation  
- `Phase3_Clustering_Analysis.ipynb` ← Notebook for K-Means clustering, PCA visualization, and cluster-label analysis  
- `CEAS_08.csv` ← Original phishing email dataset  
- `artifacts/` ← Folder containing saved TF-IDF vectorizer, scaler, and feature data files  
- `Phase2_Model_Training.ipynb` ← Notebook for models training and evaluation  
- `README.md` ← Project documentation and team details
