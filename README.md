# PRODIGY_GA_04

## Image-to-Image Translation using Pix2Pix

### Overview

This project demonstrates image-to-image translation using Pix2Pix, a Conditional Generative Adversarial Network (cGAN).

The model was trained on the Facades Dataset, where architectural label maps are translated into realistic building facade images. Pix2Pix learns the mapping between structured input images and corresponding real-world photographs through adversarial training.

---

## Project Objective

Generate realistic building facade images from semantic label maps using the Pix2Pix image-to-image translation framework.

---

## Dataset

### Facades Dataset

The Facades Dataset contains paired images:

- Input Image: Semantic facade labels
- Target Image: Real building photographs

Dataset Structure:

- Train Images: 400
- Test Images: 106

---

## Technologies Used

- Python
- TensorFlow
- Keras
- Google Colab
- Pix2Pix (Conditional GAN)

---

## Model Architecture

### Generator

The Generator uses a U-Net architecture with skip connections to preserve spatial information while generating realistic facade images.

### Discriminator

The Discriminator uses a PatchGAN architecture that classifies local image patches as real or fake, improving image quality and structural consistency.

---

## Training

The model was trained for 25 epochs on the Facades Dataset.

Training Loss Examples:

- Generator Loss: 29.60
- Discriminator Loss: 0.30

The Generator progressively learned facade structures, windows, floors, and architectural layouts from semantic maps.

---

## Results

The trained Pix2Pix model successfully generated building facade images from semantic label maps.

Although fine image details remain blurred due to limited training epochs, the model learned overall building structures, window placements, and facade layouts.

---

## Screenshots

### Dataset Sample

![Dataset Sample](screenshots/dataset_sample.png)

### Generator Architecture

![Generator](screenshots/generator_architecture.png)

### Training Logs

![Training](screenshots/training_logs.png)

### Prediction Result

![Prediction](screenshots/prediction_result.png)

---

## Repository Structure

PRODIGY_GA_04
│
├── screenshots/
│   ├── dataset_sample.png
│   ├── generator_architecture.png
│   ├── training_logs.png
│   └── prediction_result.png
│
├── .gitignore
├── PRODIGY_GA_04_Pix2Pix.ipynb
├── requirements.txt
├── README.md
└── LICENSE

---

## Internship Information

Completed as part of the Generative AI Internship Program at Prodigy InfoTech.
