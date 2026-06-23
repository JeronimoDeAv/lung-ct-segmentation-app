# Lung CT Segmentation using Deep Learning

This project explores the application of deep learning for automatic lung segmentation from chest CT images. Two different approaches were implemented and compared: a U-Net model developed from scratch and a Transfer Learning model using a pre-trained VGG16 encoder.

The project also includes a Streamlit application that allows users to upload CT images, select a segmentation model and visualize the generated prediction through an interactive interface.

Developed as the final project for the Digital Image Processing course at Pontificia Universidad Javeriana Cali.

---

## Overview

Manual segmentation of chest CT images is a time-consuming process that requires significant expertise. This project investigates whether deep learning models can automate this task while maintaining accurate segmentation of lung structures.

Two different architectures were implemented and evaluated under the same training conditions. The first model consists of a U-Net architecture built from scratch, while the second uses Transfer Learning with a pre-trained VGG16 encoder. To demonstrate a practical application of both models, they were deployed in a Streamlit web application designed for an intuitive clinical workflow.

---

## Features

- Automatic lung segmentation from chest CT images
- U-Net implementation developed from scratch
- Transfer Learning model using VGG16
- Interactive Streamlit interface
- Patient information registration
- Segmentation visualization
- Performance metrics visualization
- Downloadable prediction results

---

## Deep Learning Models

### U-Net

A U-Net architecture was implemented from scratch and trained for binary lung segmentation using chest CT images.

### Transfer Learning

A second architecture was developed using a pre-trained VGG16 encoder integrated into the U-Net framework. This approach allowed the model to leverage previously learned visual features and provided more stable training on a limited dataset.

---

## Application

The Streamlit application allows users to:

- Register patient information.
- Upload a chest CT image.
- Select one of the available segmentation models.
- Generate segmentation predictions.
- Compare model outputs.
- Download the resulting segmentation.

The application was designed as a proof of concept showing how deep learning models can be integrated into an intuitive interface for healthcare professionals.

---

## Technologies

- Python
- TensorFlow
- Keras
- Streamlit
- OpenCV
- NumPy
- Matplotlib

---

## Repository Structure

```text
lung-ct-segmentation/
│
├── app.py
├── model_handler.py
├── image_processor.py
├── history_handler.py
├── history_loader.py
├── metrics.py
├── requirements.txt
└── README.md
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/<username>/lung-ct-segmentation.git
```

Install the required packages

```bash
pip install -r requirements.txt
```

Run the application

```bash
streamlit run app.py
```

---

## Results

Both approaches successfully performed lung segmentation on chest CT images. The Transfer Learning model showed more stable training behavior and generally produced more consistent segmentation masks than the U-Net model trained from scratch. The Streamlit application demonstrates how both models can be deployed in an accessible interface for practical use.

---

## Authors

Jerónimo Delvasto Ávila

Stefanía Bravo Guzmán

Biomedical Engineering

Pontificia Universidad Javeriana Cali
