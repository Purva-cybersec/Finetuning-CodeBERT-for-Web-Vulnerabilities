# Finetuning CodeBERT for Web Vulnerabilities

## Project Overview
This project focuses on fine-tuning CodeBERT to classify text descriptions of web vulnerabilities, such as SQL Injection and Cross-Site Scripting (XSS). The goal is to automate the detection of vulnerabilities in text-based code descriptions to enhance cybersecurity measures.

## Group Members
- **Purva Naresh Rumde**
- **Sanchith Venkatesan**

*Special thanks to my partner, Sanchith Venkatesan, for their invaluable collaboration in this project.*

## Introduction
Web vulnerabilities like SQL Injection and XSS pose significant security risks to applications. Automating their detection in textual descriptions can aid in early prevention of security breaches. This project utilizes CodeBERT, a pre-trained language model, for classification tasks specific to cybersecurity.

## Problem Statement
Web vulnerabilities often lead to unauthorized access or data breaches. Identifying these vulnerabilities in textual descriptions is crucial for securing applications. This project aims to train a machine learning model to classify text-based descriptions of common vulnerabilities accurately.

## Methodology
### Dataset
- **Source:** National Vulnerability Database (NVD) by NIST
- **Format:** JSON structured data containing recent CTF challenges.

### Vulnerabilities Covered
- SQL Injection
- Cross-Site Scripting (XSS)
- Command Injection
- Directory Traversal

### Preprocessing
- Data was split into an 80-20 train-test ratio.
- Tokenization and padding were applied to standardize input formats.

### Model
- **Base Model:** CodeBERT (pre-trained by Microsoft for code-related tasks).
- **Training Setup:**
  - Three epochs
  - Evaluation after each epoch
  - Metrics: Accuracy and F1-Score

### Tools Used
- Jupyter Notebooks
- LinProg server for training (due to hardware limitations).

## Results
- Training loss decreased significantly across three epochs.
- Accuracy improved from 90.2% to 94.0%.
- F1-Score increased from 0.86 to 0.914, demonstrating better precision and recall balance.
- Successfully classified text snippets for SQL Injection, XSS, Command Injection, and Directory Traversal.

## Key Observations
- The model performed well in detecting vulnerabilities but struggled with multi-class vulnerabilities in a single text snippet.
- Fine-tuning CodeBERT on domain-specific datasets proved effective for cybersecurity applications.

## Conclusion
This project demonstrates the potential of machine learning models like CodeBERT in automating the detection of web vulnerabilities. Despite hardware limitations, the model achieved high accuracy and reliability, showcasing its utility in cybersecurity.

## Disclaimer
This project was conducted in a controlled environment for research purposes only. Proper precautions were taken to ensure the ethical handling of sensitive data.
