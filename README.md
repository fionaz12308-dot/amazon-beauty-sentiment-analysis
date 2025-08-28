# amazon-beauty-sentiment-analysis
A comprehensive sentiment analysis of Amazon Beauty product reviews using NLP and Machine Learning.


## Project Overview
This project performs a comprehensive sentiment analysis on millions of Amazon customer reviews in the "Beauty and Personal Care" category. Utilizing Natural Language Processing (NLP) and Machine Learning techniques, it aims to uncover the factors driving consumer satisfaction and provides actionable insights for brands.

**Core Objectives:**
1.  **Model Comparison:** Compare the performance of Logistic Regression, Random Forest, and VADER in sentiment classification tasks.
2.  **Factor Analysis:** Investigate the impact of product **price**, **brand**, and **color** on review sentiment.
3.  **Keyword Insight:** Identify the most frequent words and phrases associated with positive and negative experiences.

**Dataset:** Over 23 million reviews from the [Amazon Review Data ]https://huggingface.co/datasets/McAuley-Lab/Amazon-Reviews-2023

## 🛠Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, NLTK, VADER, Matplotlib, Seaborn
- **Environment:** Google Colab, Jupyter Notebook
- **Key Techniques:** TF-IDF Vectorization, SMOTE for Imbalance Handling, Hypothesis Testing

##  Key Steps & Findings
1.  **Data Processing:** Cleaned 23M+ reviews, extracted key features (`brand`, `color`), and filtered for `verified_purchase` only.
2.  **Handling Class Imbalance:** Addressed the extreme skew in ratings (J-shaped distribution) using the **SMOTE** algorithm, significantly improving model performance on negative reviews.
3.  **Model Performance:** **Logistic Regression** achieved the best balance (Accuracy: 88.58%, F1-Score for Negative Class: 0.76), outperforming Random Forest and the rule-based VADER model in overall negative sentiment detection.
4.  **Business Insights:**
    -   A strong positive correlation between **product price** and positive sentiment was found.
    -   Specific **colors** (e.g., "Washable Black Brown") had a significantly higher proportion of negative reviews (>30%).
    -   The term **"color"** appeared in both top positive and negative keywords, indicating it is a polarizing feature for consumers.

##  Results Summary (Table)
| Model | Accuracy | ROC AUC | F1-Score (Negative) | F1-Score (Positive) |
| :--- | :---: | :---: | :---: | :---: |
| Logistic Regression | 88.58% | 0.951 | 0.76 | 0.92 |
| Random Forest | 81.56% | 0.894 | 0.64 | 0.88 |
| VADER (Rule-based) | 88.77% | N/A | 0.67 | 0.93 |

## 👨‍💻 Author
**Fiona Zi**
