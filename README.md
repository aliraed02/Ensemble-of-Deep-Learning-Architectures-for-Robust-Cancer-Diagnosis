# Ensemble of Deep Learning Architectures for Robust Cancer Diagnosis

## Overview
This project is dedicated to robust cancer diagnosis through the utilization of an ensemble of deep learning architectures. The primary objective is to create an efficient and accurate system capable of identifying various types of cancer from medical images. The ensemble consists of models specifically tailored for oral, brain, breast, cervical, lung, and lymphoma cancers.

## Dataset
The dataset used for training and evaluation can be accessed [here](www.kaggle.com/datasets/obulisainaren/multi-cancer). Please download the dataset before running the code.

## Preprocessing
The preprocessing phase involves the following essential steps:

1. **Data Cleaning:** Elimination of duplicate images and resizing for consistency.
2. **Data Splitting:** Stratified sampling ensures a representative distribution in the training and testing datasets.

## Models
The system incorporates different models, each designed for specific cancer types. The models vary in the number of convolutional neural network (CNN) layers:

- **Two Layers of CNN:**
    - Oral Cancer Model
- **Three Layers of CNN:**
    - Image Origin Model (IOM)
    - Brain Cancer Model
    - Breast Cancer Model
    - Lymphoma Cancer Model
- **Four Layers of CNN:**
    - Cervical Cancer Model
    - Lung Cancer Model

## System Workflow
The system follows a sequential process to ensure efficient resource utilization and accurate classification:

### Preprocessing Pipeline:
1. Images are resized to a standardized 128x128 dimensions.
2. Rescaling is applied to normalize pixel values, bringing them within the 0 to 1 range.

### Image Origin Model (IOM):
1. The preprocessed image is fed into the IOM to determine the most suitable classification model to employ.
2. This step is implemented to optimize resource utilization.

### Classification Model:
1. The identified cancer-specific model (oral, brain, breast, cervical, lung, or lymphoma) is invoked to perform the final classification task.

By implementing this ensemble approach, the system aims to enhance the overall robustness and accuracy of cancer diagnosis, providing a reliable tool for medical professionals. Feel free to reach out if additional details or clarifications are needed.
