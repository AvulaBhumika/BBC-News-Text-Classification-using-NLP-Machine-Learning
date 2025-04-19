## BBC News Text Classification using NLP & Machine Learning

![image](https://github.com/user-attachments/assets/64859715-866e-4c36-b32e-b58594d34b06)


###  Overview
This project focuses on **automatically classifying BBC news articles** into predefined categories using Natural Language Processing (NLP) and machine learning techniques. The goal is to build a robust text classification model capable of accurately predicting the **category of unseen articles**.

---

###  Dataset Description

- **Train.csv** and **Test.csv** files contain:
  - `ArticleId`: Unique ID for each article
  - `Text`: News article content
  - `Category`: Target label (only in train)

- **Submission Format**:
  - Columns: `ArticleId`, `Category`
  - Must predict `Category` for each article in test set

---

###  Categories
The dataset includes the following news categories:
- `business`
- `entertainment`
- `politics`
- `sport`
- `tech`

---

### Project Pipeline

#### 1. **Text Preprocessing**
- Lowercasing
- Removing punctuation and digits
- Tokenization
- Stopword removal
- Lemmatization

#### 2. **Exploratory Data Analysis (EDA)**
- Distribution of categories
- Article length analysis

#### 3. **Feature Engineering**
- TF-IDF Vectorization

#### 4. **Model Training & Evaluation**
- Logistic Regression

#### 5. **Model Evaluation**
- Accuracy, Precision, Recall, F1-Score 
- Confusion Matrix
- Cross-validation
  
  ![image](https://github.com/user-attachments/assets/72713b58-9936-4f35-b230-25e92b6c50f2)


Evaluation Metrics on Validation Set:

* Accuracy : 0.9732

* Precision: 0.9735

* Recall   : 0.9732

* F1-Score : 0.9730

#### 6. **Prediction & Submission**
- Inference on `test.csv`
- Submission file generated with `ArticleId`, `Category`

---

###  Libraries Used
```text
pandas, numpy, matplotlib, seaborn, sklearn, nltk, re, string
```

### 🔮 Future Enhancements
- BERT embeddings with HuggingFace Transformers
- Streamlit/Gradio web app for interactive demo
- Multilingual classification

---

### 📎 License
This project is open-source under the MIT License.
