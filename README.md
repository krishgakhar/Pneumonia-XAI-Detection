# Pneumonia-XAI-Detection
🫁 Pneumonia Detection Using Deep Learning & Explainable AI (XAI)

This project uses fine-tuned transfer learning to classify chest X-ray images as Normal or Pneumonia, and applies Explainable AI techniques such as Grad-CAM, SHAP, and LIME to interpret model predictions.

All code, training, visualizations, and explainability outputs are contained inside the Jupyter Notebook:

📄 pneumonia_xai.ipynb
(Open directly on GitHub — it renders automatically.)

🚀 Project Highlights
🔹 Fine-Tuned Transfer Learning

Uses a pretrained CNN (e.g., VGG/ResNet/DenseNet)

Freezes base layers initially

Unfreezes top layers for fine-tuning

Uses very low learning rate to avoid overwriting pretrained weights

🔹 Dataset

Chest X-Ray Pneumonia Dataset
(Normal + Pneumonia classes)

Dataset Source:
https://data.mendeley.com/datasets/rscbjbr9sj/2

🔹 Image Preprocessing

Convert to RGB

Resize to model input size

Normalize pixel values

Expand dimensions for batch prediction

🧠 Explainable AI (XAI) Used
⭐ 1. Grad-CAM

Generates heatmaps showing lung regions influencing prediction

Highlights infection areas in pneumonia X-rays

⭐ 2. LIME

Breaks image into superpixels

Tests importance of each region

Useful when Grad-CAM fails or to cross-validate results

⭐ 3. SHAP

Provides pixel-level contribution values

Shows which parts of the X-ray push prediction toward NORMAL or PNEUMONIA

More mathematically rigorous (Shapley values)

📊 Model Evaluation

The notebook includes:

Training and validation accuracy/loss

Sample predictions

Grad-CAM heatmaps

SHAP plots

LIME explanations
