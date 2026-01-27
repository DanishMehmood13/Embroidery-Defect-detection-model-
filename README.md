🧵 Embroidery Defect Detection using Mask R-CNN
📌 Overview

In the textile and garment industry, embroidery quality inspection is traditionally performed manually by human inspectors. This process is time-consuming, subjective, and prone to human error—especially when dealing with complex embroidery patterns and high production volumes.

This project presents an AI-based computer vision system that automates embroidery quality inspection by detecting and segmenting defects at the pixel level using Mask R-CNN.

❓ Problem Statement

Manual inspection of embroidered fabrics suffers from:

Human fatigue and inconsistency

Difficulty in identifying small or overlapping defects

Lack of scalability for industrial production

The objective of this project is to automate embroidery defect detection and provide accurate, consistent, and scalable quality control.

🎯 Objectives

Detect embroidery defects such as missing stitches and overlaps

Localize defects using instance segmentation

Reduce dependency on manual inspection

Build a foundation for advanced transformer-based models

🧠 Methodology

The problem is formulated as an instance segmentation task.

Key Techniques Used:

Mask R-CNN for pixel-level defect segmentation

Detectron2 framework

Custom annotated dataset (images + masks)

CNN-based backbone for local feature extraction

Each defect instance is detected, classified, and segmented to clearly highlight defective regions in embroidered fabric.

🗂 Dataset

Custom dataset created for embroidery defect detection

Images paired with corresponding binary masks

Dataset split into training and validation sets

Supports defects like:

Missing embroidery

Overlapping stitches

⚠️ Dataset is research-oriented and prepared specifically for this project.

📁 Project Structure
embroidery-defect-detection/
│
├── datasets/
│   ├── train/
│   ├── val/
│
├── annotations/
│   ├── train.json
│   ├── val.json
│
├── configs/
│   └── mask_rcnn_config.yaml
│
├── train.py
├── inference.py
├── utils/
│
├── results/
│   └── sample_predictions/
│
└── README.md

⚙️ Installation
pip install -r requirements.txt


Make sure you have:

Python 3.8+

PyTorch

Detectron2

OpenCV

NumPy

🚀 Training
python train.py

🔍 Inference
python inference.py


The output will include segmentation masks overlaid on embroidery images highlighting defective regions.

📊 Results

Accurate localization of embroidery defects

Pixel-level segmentation using Mask R-CNN

Clear visual distinction between normal and defective embroidery regions

Sample results are available in the results/ directory.

🔮 Future Work

Integrate Swin Transformer to capture global contextual information

Improve performance on complex and repetitive embroidery patterns

Optimize model for real-time industrial deployment

🏭 Applications

Textile manufacturing quality control

Automated inspection systems

Smart factories and Industry 4.0 solutions

🙌 Acknowledgments

Detectron2 by Facebook AI Research

Open-source computer vision community

📬 Contact

If you have questions or would like to collaborate, feel free to connect with me on LinkedIn or GitHub.
