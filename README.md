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

## Severity Classes

- Mild
- Moderate
- Severe
  
## Installation

### Prerequisites

- Python 3.8 or later
- TensorFlow 2.15 or later
- OpenCV
- NumPy
- scikit-learn
- Matplotlib
- Transformers (HuggingFace)

### Installation Steps

```bash
git clone https://github.com/PoorniKR/Rice-Leaf-Disease.git
cd Rice-Leaf-Disease
pip install -r requirements.txt
```

## Results

- Achieved 94.41% classification accuracy on the test set.
- Grad-CAM outputs highlight infected regions, which are clustered to estimate severity.
- The system can handle difficult classes like Tungro and Neck Blast with robust performance.

## Output

<img width="1920" height="1080" alt="3" src="https://github.com/user-attachments/assets/6e0395d7-4984-44d8-a481-2463ef494fba" />
<img width="1920" height="1080" alt="2" src="https://github.com/user-attachments/assets/005bc943-2de1-41fb-bb3a-915ae6a34575" />
<img width="1920" height="1080" alt="1" src="https://github.com/user-attachments/assets/750897ef-56c2-4212-8939-59facfb68a81" />
