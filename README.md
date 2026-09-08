# Music Genre Classification

## Overview
This project was developed as the final assignment for the Selected Topics in Music and Acoustic Engineering course of the master’s degree in music and Acoustic Engineering at Politecnico di Milano.
The objective is to automatically classify music tracks into their corresponding genres using both classical machine learning and deep learning approaches.
The project implements the complete Music Information Retrieval (MIR) pipeline, including audio preprocessing, feature extraction, model training, and performance evaluation.

## Dataset
The project uses the Free Music Archive (FMA Small) dataset together with the corresponding metadata (the dataset is not included in this repository).

## Methodology
1. Audio preprocessing
* Audio loading with Librosa
* Standard sampling rate (22.05 kHz)
* Duration normalization (30 seconds)
* Metadata association using the FMA dataset

2. Feature extraction
Several complementary MIR features are extracted:
* Mel Spectrograms
* MFCCs
* Spectral Centroid
* Zero Crossing Rate
* Chroma Features
* Tempogram
Two feature representations are generated:
* Handcrafted feature vectors for classical machine learning
* Mel spectrograms for convolutional neural networks

3. Data preprocessing
* Stratified train/validation/test split
* Label encoding
* Feature standardization using StandardScaler

4. Machine Learning models
The following classifiers are implemented and compared:
* Random Forest
* Support Vector Machine (RBF kernel)
* Multi-Layer Perceptron (MLP)
* Convolutional Neural Network (CNN)

5. Evaluation
Each model is evaluated using:
* Classification accuracy
* Classification report
* Confusion matrix
(results in report)

## Authors
* Antonio Treviglio
* Eleonora Berra
* Federico Giacopuzzi
* Tekla Gizella Kalmár

Master’s degree in Music and Acoustic Engineering  
Politecnico di Milano





