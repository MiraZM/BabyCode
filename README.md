# BabyCode Project 

## 1.0 Introduction

Welcome to BabyCode, where technology meets compassion in decoding the language of baby cries. BabyCode is more than just a project; it's a mission to empower parents, especially mothers, by translating infant cries into understandable insights. Our mobile application aims to strengthen the bond between parents and babies, ensuring no cry goes misunderstood.

### Project Timeline:
- **Start Date:** 8th March 2024
- **End Date:** 25th May 2024

## 1.1 Need Analysis and Description

Meet Maya, our primary user persona, a first-time mother navigating the challenges of parenthood. Maya often struggles to interpret her baby's cries, leading to stress and uncertainty. She seeks a reliable, non-intrusive mobile application to decode these cries in real-time, providing confidence and peace of mind in her parenting journey.

## 1.2 Project Constraints

During development, we faced challenges:
- **Limited Dataset:** Initially, a small dataset of baby cries required rigorous preprocessing and feature extraction.
- **Time Constraints:** Efficient data collection and classification within a limited timeframe were crucial but challenging.

## 1.3 System Environment

BabyCode is designed as a mobile application for iOS and Android:
- **Key Features:** Real-time cry analysis and intuitive user interface for recording and interpreting baby cries.

## 1.4 Project Software and Hardware Requirements

### Software:
- **GUI Design:** Figma
- **Programming Language:** Python with libraries such as Keras and Librosa for machine learning and audio processing.

### Hardware:
- **Smartphone with Microphone:** Required for recording baby cries.
- **Internet Connection:** Necessary for app installation, updates, and model improvements.

## 2.0 Research Background and Related Works

We drew insights from various studies and papers on infant cry classification using machine learning techniques. Notable contributions include:
- Different models and techniques for cry classification.
- Use of features like MFCC, spectrograms, and CNNs for effective classification.

## 3.0 Proposed Methodology

### 3.1 Pipeline of the Proposed Methodology

Our methodology includes:
- Data collection and preprocessing.
- Feature extraction (MFCC, Mel Spectrogram, Chroma, Spectral Contrast).
- Model training using a 1D Convolutional Neural Network (CNN).
- Evaluation and deployment of the trained model.

### 3.2 Technical and Implementation Description

Detailed implementation involved:
- Dataset utilization from Donate a Cry Corpus on GitHub.
- Feature extraction using Librosa and Python.
- Training a CNN model on extracted features for cry classification.
- User-friendly GUI development using Figma and Python.

### 3.3 Dataset Description

We utilized the Donate a Cry Corpus dataset:
- **Features:** Cleaned and preprocessed with specific settings for optimal feature extraction.
- **Categories:** Categorized into 'Needs Burping', 'Belly Pain', 'Being Tired', 'Being Discomfort', and 'Being Hungry'.

### 3.4 Data Preprocessing

Minimal preprocessing was required due to dataset quality:
- Ensured audio samples were mono for consistency.
- Efficient transition to feature extraction phase.

### 3.5 Feature Extraction

Utilized multiple features:
- MFCC, Mel Spectrogram, Chroma, Spectral Contrast, and Tonnetz.
- Enhanced model performance through comprehensive feature representation.

### 3.6 Feature Selection

Selected top features using SelectKBest for model efficiency:
- ANOVA F-value scoring for feature selection.
- Training and testing dataset split for model preparation.

### 3.7 Features Classification

1D CNN model implementation:
- Sequential model construction with convolutional and pooling layers.
- Training with Adam optimizer, batch size of 64, over 100 epochs.

## 4.0 Experimental Results and Analysis

### 4.1 Performance Measures

Evaluation metrics:
- **Accuracy:** 86.09% on validation set.
- **Loss:** 0.3185 on validation set.

### 4.2 Experimental Results

The CNN model demonstrated robust performance:
- High accuracy and low loss on training and validation datasets.
- Challenges in generalization highlighted for future improvements.

## 5.0 Conclusions and Future Works

### 5.1 Strengths

- **High Accuracy:** Despite dataset limitations, achieved robust classification results.
- **Effective Feature Extraction:** MFCC and Mel Spectrogram provided rich audio representations.

### 5.2 Weaknesses

- **Dataset Size:** Limited dataset may affect model generalization.
- **Label Accuracy:** Expert validation needed for dataset labels.

### 5.3 Future Works

- Expand dataset for improved model performance.
- Collaborate with domain experts for label validation and dataset augmentation.
- Develop real-time application for continuous cry monitoring and analysis.

## Conclusion

BabyCode leverages machine learning to decode and understand baby cries, paving the way for enhanced parent-baby interactions. Our project demonstrates the potential of AI in addressing fundamental parenting challenges, underscoring the importance of technology in childcare.

---

This README provides a comprehensive overview of the BabyCode project, detailing its inception, methodology, implementation, results, and future directions. Adjust as necessary to fit the formatting and conventions of your GitHub repository.
