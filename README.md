# Cervical Cancer Classification using CNN

## Overview
This project focuses on the automated classification and identification of cervical cancer using deep learning techniques applied to liquid-based cytology (LBC) Pap smear images.

The work was completed as part of an MSc Data Science final-year project at Coventry University.

## Problem Statement
Cervical cancer remains a major global health challenge. Early and accurate detection is critical for improving patient outcomes. Manual cytological analysis is time-consuming and prone to inter-observer variability. This project explores the use of convolutional neural networks (CNNs) to assist in multi-class cervical cancer diagnosis.

## Dataset
- Source: Mendeley Data
- Total images: 963
- Classes: NIM, LSIL, HSIL, SCC

(See `data/README.md` for dataset access details)

## Models Implemented
- Custom CNN
- VGG-16
- VGG-19
- ResNet-50
- ResNet-101
- Ensemble classifier

## Tools & Technologies
- Python
- TensorFlow / Keras
- NumPy, Pandas, Matplotlib, Seaborn
- Jupyter Notebook
- GitHub

## Results
The models achieved strong classification performance, with VGG-based architectures showing the highest accuracy. Performance was evaluated using accuracy, precision, recall, and F1-score metrics.

## Repository Structure
- `notebook/` – Model training and evaluation code
- `data/` – Dataset information and access link
- `Report/` – MSc project report

## Notes
This repository demonstrates an end-to-end machine learning workflow including data preprocessing, model development, evaluation, and documentation.
