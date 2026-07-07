# Intelligent Intrusion Detection System Using the CIC-IDS-2017 Dataset

A Machine Learning-based Intrusion Detection System (IDS) developed using the CIC-IDS-2017 dataset to detect and classify malicious network traffic with high accuracy. This project evaluates multiple supervised machine learning algorithms and demonstrates that classical ensemble learning methods can effectively identify cyberattacks while maintaining excellent computational efficiency.

---

# Project Overview

Cybersecurity threats continue to evolve rapidly, making traditional signature-based intrusion detection systems less effective against modern attacks. Organizations require intelligent systems capable of identifying both known and previously unseen malicious network behavior.

This project develops an intelligent Intrusion Detection System (IDS) using supervised machine learning techniques. The system is trained on the CIC-IDS-2017 dataset, one of the most widely used benchmark datasets in cybersecurity research.

The project focuses on:

- Data preprocessing and cleaning
- Handling highly imbalanced attack classes
- Training multiple machine learning models
- Performance comparison of different algorithms
- Identifying the best-performing model based on accuracy and efficiency

---

# Problem Statement

Traditional intrusion detection systems rely heavily on predefined attack signatures. Although effective against known attacks, they struggle to detect:

- Zero-day attacks
- Advanced persistent threats (APTs)
- Sophisticated network intrusions
- Rare attack patterns

The objective of this project is to develop an intelligent machine learning-based intrusion detection system capable of accurately classifying benign and malicious network traffic while minimizing false positives and false negatives.

---

# Objectives

The primary objectives of this project include:

- Build an intelligent network intrusion detection model.
- Perform preprocessing and feature engineering on network traffic data.
- Handle class imbalance within the dataset.
- Compare the performance of multiple supervised machine learning algorithms.
- Evaluate model performance using standard classification metrics.
- Identify the most accurate and computationally efficient algorithm.

---

# Dataset

**Dataset:** CIC-IDS-2017

The CIC-IDS-2017 dataset was developed by the Canadian Institute for Cybersecurity (CIC) and contains realistic network traffic captured over five days.

The dataset includes both normal traffic and numerous attack scenarios that closely resemble real-world cyberattacks.

### Dataset Characteristics

- Approximately 2.8 million network flow records
- 79 network traffic features
- 15 traffic classes
- Realistic network simulation
- Fully labeled attack categories

### Attack Categories

- BENIGN
- DDoS
- DoS Hulk
- DoS GoldenEye
- DoS Slowloris
- DoS SlowHTTPTest
- FTP-Patator
- SSH-Patator
- PortScan
- Botnet
- Web Attack – Brute Force
- Web Attack – SQL Injection
- Web Attack – XSS
- Infiltration
- Heartbleed

---

# Data Preprocessing

The dataset underwent several preprocessing steps before model training.

### Data Cleaning

- Merged multiple CSV files
- Removed duplicate records
- Removed missing values
- Replaced infinite values
- Standardized feature names

### Data Balancing

The original dataset was highly imbalanced, with benign traffic dominating the dataset.

To improve model performance:

- Majority classes were downsampled
- Rare attack classes were retained
- Final balanced dataset contained approximately 190,000 network flows

---

# Machine Learning Models

The following supervised machine learning algorithms were implemented and compared:

- Random Forest
- Extra Trees Classifier
- Decision Tree
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes
- Multi-Layer Perceptron (MLP Neural Network)

Each model was trained using default Scikit-learn parameters to ensure a fair comparison.

---

# Model Evaluation Metrics

Performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

---

# Results

Among all evaluated models, ensemble tree-based algorithms consistently achieved the highest performance.

## Best Performing Model

**Random Forest Classifier**

### Performance

- Accuracy: **99.24%**
- Excellent detection of both common and rare attacks
- Low false positive rate
- Fast training time
- Highly reliable for network intrusion classification

The experimental results demonstrate that classical ensemble learning algorithms outperform more computationally expensive neural network approaches for this dataset.

---

# Technologies Used

Programming Language

- Python

Libraries

- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

Development Environment

- Google Colab
- Jupyter Notebook

---

# Repository Structure

```
intrusion-detection-cic-ids-2017/
│
├── Prog_found.ipynb
├── prog_found_ppt.pptx
├── CIC Intrusion Detection Datasets.html
└── README.md
```

---

# Future Enhancements

Potential improvements include:

- Real-time intrusion detection
- Deep learning models (CNN, LSTM)
- Feature selection and dimensionality reduction
- Hyperparameter optimization
- Deployment using Flask or Streamlit
- Live packet capture using Scapy
- Cloud deployment for production environments

---

# References

- Sharafaldin, I., Lashkari, A. H., & Ghorbani, A. A. (2018). *Toward Generating a New Intrusion Detection Dataset and Intrusion Traffic Characterization.*
- Canadian Institute for Cybersecurity (CIC)
- Scikit-learn Documentation

---

# Author

## Rohini Muniganti

**Master of Science in Computer Science**  
University of Central Missouri

GitHub: https://github.com/Rohini786

---

# License

This project is intended for academic research and educational purposes.
