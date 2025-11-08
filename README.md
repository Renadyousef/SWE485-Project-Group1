# Spam Email Detection – SWE485


##  Why We Chose This Topic
We chose this project because phishing and spam emails are one of the most common cybersecurity threats today.  
Being able to automatically detect them helps protect users and organizations from scams and data leaks.

---

###  Team Members

| Name | Student ID |
|------|-------------|
| fajer alkatheri        | [443204563] | 
| renad alotibi          | [443200801]  | 
| rawan khaled           | [443204623] | 
| rahaf samkari          | [443202844] | 
| Salha Abdullah Shahbal | 443204567   | 


---
### Dataset
- Source: [Phishing Email Dataset on Kaggle](https://www.kaggle.com/datasets/naserabdullahalam/phishing-email-dataset)  
- Contains around 39,000 emails labeled as *Spam (1)* or *legitimate (0)*.  
- Key columns include:  
  - subject, body: email text  
  - urls, receiver_spam_ratio :[extracted], capital_ratio: extracted numeric features and more ..
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
###  What We Did in Phase 2
in this phase we did :
- split the data into train,test
- trained 3 models
- evaluted them 
- chose the best fit
- captured the high weight features in text
- analyzed whats wrong and applied erorr analysis (underfit,overfit,good fit) and removed highly coroleted column (cheating column)
---

### files in This Repository 

Phase1_Data_Exploration.ipynb   ← notebook for data exploration, feature extraction, and TF-IDF transformation  
CEAS_08.csv                     ← Original phishing email dataset  
  
artifacts/                      ← Cleaned data Folder 
containing saved TF-IDF vectorizer, scaler, and feature data files  
phase 2   ← notebook for models training and evaluation 
README.md                       ← Project documentation and team details
