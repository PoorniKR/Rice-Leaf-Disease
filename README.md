# Rice Leaf Disease Detection and Severity Estimation

This project focuses on the identification and severity estimation of rice leaf diseases using a deep learning-based hybrid approach. It combines image preprocessing, segmentation, hybrid feature extraction, and Grad-CAM-based unsupervised severity prediction to assist in precision agriculture.

## Project Description

Rice crops are susceptible to several diseases that affect crop health and reduce yield. This system:

- Detects and classifies multiple rice leaf diseases.
- Estimates the severity of the infection without labeled severity data.
- Provides visual explanations through Grad-CAM.
- Can be extended into a mobile application for use by farmers and agronomists.

## Features

- Image preprocessing using contrast enhancement (CLAHE), bilateral filtering, and edge detection.
- Disease region segmentation using Adaptive Gaussian Thresholding and Adaptive Fuzzy C-Means (AFCM).
- Local and global feature extraction using InceptionResNetV2 and Vision Transformer (ViT).
- Weighted feature fusion (70% InceptionResNetV2 + 30% ViT).
- Disease classification using dense neural networks.
- Unsupervised severity estimation using Grad-CAM and clustering.

## Disease Classes

- Bacterial Leaf Blight
- Brown Spot
- Leaf Blast
- Narrow Brown Spot
- Leaf Scald
- Sheath Blight
- Tungro
- Rice Hispa
- Neck Blast

## Installation

### Prerequisites

- Python 3.8 or later
- TensorFlow 2.9 or later
- OpenCV
- NumPy
- scikit-learn
- Matplotlib
- TensorFlow Addons
- Transformers (HuggingFace)

### Installation Steps

```bash
git clone https://github.com/PoorniKR/rice-leaf-disease-detection.git
cd rice-leaf-disease-detection
pip install -r requirements.txt

