# Classification and identification of cervical cancer using CNN methods 

## Overview
This project focuses on the classification and identification of cervical cancer using deep learning techniques applied to liquid-based cytology (LBC) Pap smear images. Cervical cancer is one of the leading causes of cancer-related deaths among women worldwide, and early, accurate detection plays a critical role in improving patient outcomes.

The project develops an automated multi-class diagnostic system using convolutional neural networks (CNNs) and transfer learning to classify cervical cell abnormalities. The objective is to support medical screening workflows by improving diagnostic consistency, reducing manual effort, and enabling scalable image-based analysis.
The work was completed as part of an MSc Data Science final-year project at Coventry University.

## Problem Statement
Cervical cancer remains a major global health challenge. Early and accurate detection is critical for improving patient outcomes. Manual examination of Pap smear images is time-intensive, subjective, and highly dependent on expert interpretation, which can lead to inter-observer variability and delayed diagnosis. Even with liquid-based cytology providing improved image quality, accurate classification of cervical abnormalities remains challenging, especially when handling large volumes of samples.

The core problem addressed in this project is the lack of an automated and reliable multi-class classification system capable of accurately distinguishing between normal, pre-cancerous, and cancerous cervical cell types. The goal is to leverage deep learning models to enhance screening accuracy, reduce diagnostic errors, and assist decision-making in cervical cancer detection.

## Dataset
- Source: Mendeley Data

The project uses a publicly available cervical cancer dataset from Mendeley Data, consisting of 963 liquid-based cytology Pap smear images collected from 460 patients. The images were captured at 40× magnification and labeled by expert cytologists according to the Bethesda classification system.

Classes:

Negative Intraepithelial Malignancy (NIM) – 613 images

High Squamous Intraepithelial Lesion (HSIL) – 163 images

Low Squamous Intraepithelial Lesion (LSIL) – 113 images

Squamous Cell Carcinoma (SCC) – 74 images

The dataset exhibits class imbalance, reflecting real-world clinical conditions. Due to licensing and size constraints, the dataset is referenced via an external link rather than being hosted directly in this repository.

(See `data/README.md` for dataset access details)

## Models Implemented
Several deep learning architectures were implemented and compared for multi-class image classification:

- Custom Convolutional Neural Network (CNN)
- VGG-16 (transfer learning with fine-tuning)
- VGG-19 (transfer learning with fine-tuning)
- ResNet-50
- ResNet-101
- Ensemble Classifier

To address limited dataset size and improve generalization, transfer learning was applied using pre-trained ImageNet weights. Additionally, an ensemble classification approach was developed by combining predictions from top-performing models to improve robustness and classification performance.
 

## Tools & Technologies

- Programming Language: Python
- Deep Learning Frameworks: TensorFlow, Keras
- Data Processing & Visualization: NumPy, Pandas, Matplotlib, Seaborn
- Modeling Techniques: CNNs, Transfer Learning, Ensemble Learning
- Development Environment: Jupyter Notebook, Google Colab (GPU-enabled)
- Version Control: GitHub

These tools enabled efficient experimentation, training, and evaluation of deep learning models on medical image data.

## Results

Model performance was evaluated using accuracy, precision, recall, and F1-score, with particular emphasis on minimizing false negatives due to clinical importance.

Key Results:

- VGG-16 and VGG-19 achieved the highest classification accuracy (~94%), outperforming deeper residual networks.
- ResNet-101 achieved approximately 80% accuracy, with ResNet-50 performing slightly lower.
- The ensemble model improved prediction stability and robustness across classes.
- Deep learning models significantly outperformed traditional machine learning approaches for this task.
- These results demonstrate the effectiveness of transfer-learning-based CNN models for cervical cancer classification using LBC Pap smear images.

## Repository Structure
- `notebook/` – Model training and evaluation code
- `data/` – Dataset information and access link
- `Report/` – MSc project report

## Notes

This project demonstrates an end-to-end machine learning workflow, including data preprocessing, model training, evaluation, documentation, and comparative analysis.

The system is designed as a decision-support tool and is not intended to replace clinical diagnosis.

Future enhancements could include larger datasets, class imbalance handling, explainable AI techniques, and real-world clinical validation.

The approach can be extended to other medical imaging classification problems.
