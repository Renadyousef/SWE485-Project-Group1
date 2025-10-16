# Phishing Email Detection – SWE485


##  Why We Chose This Topic
We chose this project because phishing and spam emails are one of the most common cybersecurity threats today.  
Being able to automatically detect them helps protect users and organizations from scams and data leaks.

---

###  Team Members

| Name | Student ID | Role |
|------|-------------|------|
| fajer alkatheri        | [443204563] | Data Cleaning & Handling Missing Values|
| renad alotibi          | [44320080]  | Feature Extraction and Engineering |
| rawan khaled           | [443204623] | Text Preprocessing |
| rahaf samkari          | [443202844] | Text Preprocessing |
| Salha Abdullah Shahbal | 443204567   | Text Representation (Vectorization)|


---
### Dataset
- Source: [Phishing Email Dataset on Kaggle](https://www.kaggle.com/datasets/naserabdullahalam/phishing-email-dataset)  
- Contains around 39,000 emails labeled as *phishing (1)* or *legitimate (0)*.  
- Key columns include:  
  - subject, body: email text  
  - urls, receiver_spam_ratio, capital_ratio: extracted numeric features  
  - label: target variable

---

###  What We Did in Phase 1
In this phase, we:
- Cleaned the dataset and handled missing values.  
- Extracted new useful features from the emails.  
- Processed the text data and converted it into numerical form using *TF-IDF*.  
- Scaled the numeric features and combined them with the text vectors.  
- Saved all processed data for the next phase (model training).

---

### files in This Repository

Phase1_Data_Exploration.ipynb   ← Main notebook for data exploration, feature extraction, and TF-IDF transformation  
CEAS_08.csv                     ← Original phishing email dataset  
cleaned_CEAS_08.csv             ← Cleaned version after preprocessing and removing duplicates  
artifacts/                      ← Folder containing saved TF-IDF vectorizer, scaler, and feature data files  
README.md                       ← Project documentation and team details
