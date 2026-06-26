# Brain Tumor Segmentation in MRI Images using U-Net

Implementation of a U-Net based deep learning model for brain tumor segmentation in MRI images using TensorFlow and Keras.

This project focuses on semantic segmentation of tumor regions from MRI scans using Convolutional Neural Networks (CNNs) and the U-Net architecture.

---

# Overview

Brain tumor segmentation is an important medical imaging task used for identifying tumor regions in MRI scans.

In this project:
- MRI images are preprocessed
- Tumor masks are generated
- U-Net architecture is implemented
- Segmentation masks are predicted
- IoU metric is used for evaluation

The implementation is inspired by the research paper:

> U-Net: Convolutional Networks for Biomedical Image Segmentation

---

# Types of Brain Tumors

The dataset contains MRI scans of:
1. Meningioma
2. Glioma
3. Pituitary Tumor

---

# Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib
- Google Colab

---

# Deep Learning Concepts Used

## CNN (Convolutional Neural Network)
CNNs are used to extract spatial features from MRI images.

## Conv2D Layers
Conv2D kernels are used to detect important tumor-related patterns from MRI scans.

## U-Net Architecture
U-Net is an encoder-decoder architecture widely used for biomedical image segmentation tasks.

## Binary Segmentation
The output generated is a binary segmentation mask:
- 0 → Background
- 1 → Tumor Region

## model.fit()
Used for training the segmentation model using MRI images and masks.

## IoU (Intersection over Union)
IoU metric is used to compare predicted masks with actual masks.

## Adam Optimizer
Adam optimizer is used during model training for better convergence.

---

# Dataset

Dataset Used:
LGG MRI Segmentation Dataset from Kaggle.

The dataset contains:
- MRI images
- Tumor masks
- Brain tumor segmentation labels

---

# Project Workflow

1. Download MRI dataset
2. Preprocess MRI images
3. Normalize image data
4. Build U-Net architecture
5. Train segmentation model
6. Predict tumor masks
7. Evaluate predictions using IoU

---

# Model Architecture

The implemented U-Net architecture contains:
- Encoder path
- Bottleneck layer
- Decoder path
- Conv2D layers
- MaxPooling layers
- UpSampling layers
- Skip connections

The model is trained using:
- Binary Crossentropy Loss
- Adam Optimizer

---

# Training Output

![Training Output](screenshots/training_output.png)

---

# Loss Graph

![Loss Graph](screenshots/loss_graph.png)

---

# IoU Evaluation

![IoU Score](screenshots/iou_score.png)

---

# Model Architecture Screenshot

![Architecture](screenshots/architecture.png)

---

# Sample Outputs

## MRI Image
![MRI](samples/sample_mri.png)

## Ground Truth Mask
![Mask](samples/sample_mask.png)

## Predicted Tumor Mask
![Prediction](samples/sample_prediction.png)

---

# Files Included

```text
brain_tumor_segmentation.ipynb
download_data.sh
mat_to_numpy.py
requirements.txt
project_notes.md
project_summary.pdf