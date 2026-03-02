# 🛡 Phish Sentinel
 - An AI-Powered Browser Extension for Phishing Email Detection and Fraud Prevention
---
## Hybrid Explainable AI System for Intelligent Phishing Email Detection

Phish Sentinel is an AI-powered phishing email detection system that uses Natural Language Processing (NLP) and Machine Learning to classify emails as **Phishing** or **Legitimate**. The system provides a confidence score and explainable insights to improve transparency and user awareness.

---

# 📌 Problem Statement

Phishing emails are one of the most common cyber threats used to steal sensitive information such as passwords, banking credentials, and personal data.  

Attackers use social engineering techniques such as:
- Urgency tactics
- Fake domain names
- Credential harvesting links
- Financial targeting

Traditional spam filters often fail to detect sophisticated phishing attempts.

The challenge is to build an **NLP-based classification system** that:
- Analyzes email subject and body content
- Classifies emails as phishing or legitimate
- Provides a confidence score
- Evaluates performance using accuracy, precision, recall, and F1-score

---

# 📄 Abstract

Phish Sentinel is a hybrid machine learning-based phishing detection system designed to intelligently classify email content.  

The system applies **TF-IDF vectorization (Term Frequency-Inverse Document Frequency)** for feature extraction and uses **Logistic Regression** as the primary classifier. Additionally, a rule-based scoring mechanism enhances detection by identifying suspicious keywords and URL patterns.  

The model is trained and tested using a labeled phishing email dataset with an 80-20 train-test split. Performance is evaluated using standard classification metrics such as accuracy, precision, recall, and F1-score.  

Phish Sentinel not only detects phishing emails but also provides explainable outputs by highlighting suspicious terms, increasing transparency and user trust.

---

#  Introduction

With the rapid growth of digital communication and online financial services, phishing attacks have become increasingly prevalent. Email remains the primary attack vector for cybercriminals attempting to exploit users through deception.

Phish Sentinel aims to address this issue by leveraging Natural Language Processing and Machine Learning techniques to analyze email content. By combining statistical text representation (TF-IDF) with supervised learning (Logistic Regression), the system effectively identifies patterns associated with phishing attempts.

Unlike traditional spam filters, Phish Sentinel integrates explainable AI features to provide insights into why an email is classified as phishing. This improves usability and enhances user awareness of potential threats.

The project demonstrates a scalable and practical approach to strengthening email security using intelligent classification techniques.

## ✨ Features

- NLP-based phishing email classification
- Subject + body email analysis
- TF-IDF feature extraction
- Logistic Regression classifier
- Confidence score output
- Explainable AI (keyword highlighting)
- Model evaluation metrics (Accuracy, Precision, Recall, F1-score)

## 🛠 Tech Stack
- Python
- FastAPI
- Scikit-learn
- Pandas
- Numpy
- TF-IDF Vectorization
- Logistic Regression

## 📈 Model Evaluation

The model was evaluated using an 80-20 train-test split.

Performance Metrics:
- Accuracy : 98.26%
- Precision: 95.78%
- Recall   : 98.33%
- F1 Score : 97.04%

These metrics demonstrate strong phishing detection capability while minimizing false positives.
## 🧠 How It Works

1. Email subject and body are combined.
2. Text is cleaned and preprocessed.
3. TF-IDF converts text into numerical vectors.
4. Logistic Regression predicts phishing probability.
5. Hybrid rule-based scoring enhances detection.
6. Final classification and confidence score are generated.

## 📊 Confusion Matrix

The model demonstrates strong classification capability with low false positives and high recall.

## ⚠ Limitations

- Performance depends on dataset quality.
- May struggle with highly obfuscated phishing emails.
- Does not currently support multi-language detection.

## 🚀 Future Scope

- Integration with email clients
- Deployment using cloud services
- Deep learning models (BERT)
- Real-time threat intelligence integration

## ✅ Conclusion

Phish Sentinel presents an intelligent and scalable approach to phishing email detection using Natural Language Processing and Machine Learning techniques.

By leveraging TF-IDF feature extraction and Logistic Regression classification, the system effectively distinguishes between phishing and legitimate emails. The integration of a hybrid rule-based scoring mechanism enhances detection accuracy and provides explainable outputs through keyword highlighting and confidence scoring.

The model demonstrates strong performance across key evaluation metrics such as accuracy, precision, recall, and F1-score, ensuring reliable detection while minimizing false positives.

Overall, Phish Sentinel showcases a practical, real-world solution to combat digital fraud and strengthen email security through explainable AI-driven classification.So these are the specificarions that are used in the project to make it efficient.
