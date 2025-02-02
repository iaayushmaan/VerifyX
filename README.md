

## Problem Statement
The rapid spread of fake news and misinformation online has become a major challenge, causing confusion and harm to society. Traditional fact-checking methods are slow and cannot keep up with the volume of information shared daily. VerifyX aims to address this by providing an AI-driven solution to detect and classify fake news effectively.
## Objective
The goal of VerifyX is to build an automated system that can identify and classify fake news with high accuracy. By combining ML and DL techniques, VerifyX ensures robust and scalable fact-checking capabilities.
VerifyX is an AI-driven project designed to tackle the growing problem of fake news and misinformation online. The goal is to create a system that can automatically detect and classify fake news using advanced machine learning (ML) and deep learning (DL) techniques. The process begins with collecting and cleaning data, removing unnecessary elements like URLs and stop words, and extracting emotes and slang to better understand the tone of the text. Feature engineering is done using TF-IDF for ML models and advanced embeddings like BERT and RoBERTa for DL models. The system trains six DL models (e.g., BERT, LSTM) and five ML models (e.g., Random Forest, SVM) on both clean and perturbed data, with adversarial training using the Fast Gradient Sign Method (FGSM) to improve robustness. VerifyX aims to provide a scalable, accurate solution for fact-checking, helping social media platforms, news organizations, and governments combat misinformation effectively.

## Methodology

VerifyX follows a structured approach to detect fake news:

1. Dataset Collection: Four publicly available datasets are used for training and evaluation.

2. Preprocessing: Data is cleaned by removing URLs, usernames, hashtags, and stop words.

3. Emote and Slang Extraction: A dictionary of emotes and slang words is created, with polarity assigned to each for better tone analysis.

4. Feature Engineering:

- TF-IDF vectorization for ML models.

- Advanced embeddings (BERT, RoBERTa, DeBERTa) for DL models.

5. Model Training:

- Six DL models (BERT, RoBERTa, DeBERTa, Longformer, GRU, LSTM) and five ML models (Random Forest, Decision Tree, SVM, Naive Bayes, Logistic Regression) are trained.

- Adversarial training is performed using the Fast Gradient Sign Method (FGSM) to improve model robustness.

6. Adversarial Training: Perturbed data is generated to challenge the models, making them more reliable.

Get glove.6B.100d from here - https://drive.google.com/file/d/1QFdkeK3a3mu5at6Ocq1sxIuHzSdXl_15/view?usp=sharing

![image](https://github.com/user-attachments/assets/5ffec207-a9f9-4cc4-b575-e03b28a627bd)

## Model Performance Metrics

| Model               | Accuracy | Precision | Recall  | F1-Score |
|---------------------|----------|-----------|---------|----------|
| SVM                | 0.992650  | 0.992659  | 0.992650 | 0.992651 |
| Decision Tree      | 0.995323  | 0.995324  | 0.995323 | 0.995323 |
| Naive Bayes       | 0.927840  | 0.927858  | 0.927840 | 0.927825 |
| Random Forest      | 0.996882  | 0.996883  | 0.996882 | 0.996882 |
| Logistic Regression | 0.986526  | 0.986563  | 0.986526 | 0.986527 |
| LSTM               | 0.959354  | 0.961193  | 0.959354 | 0.959360 |
| GRU                | 0.971047  | 0.971164  | 0.971047 | 0.971053 |
| BERT-Based        | 0.968374  | 0.968399  | 0.968374 | 0.968377 |
| RoBERTa            | 0.966370  | 0.966475  | 0.966370 | 0.966376 |
| DeBERTa            | 0.943764  | 0.944176  | 0.943764 | 0.943781 |
| Longformer         | 0.435857  | 0.424461  | 0.435857 | 0.396374 |

