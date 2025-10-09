## 🔍 Overview
This directory includes experiments based on **DeepLab-V3**, a state-of-the-art semantic segmentation model used for **pixel-level fire and smoke delineation**. The model leverages atrous spatial pyramid pooling (ASPP) to capture multi-scale contextual information. All implementations utilize **torchvision.models.segmentation** with pretrained COCO weights.

## 🧩 Data Organization and Preprocessing
Before running the training scripts, please organize your dataset as follows:

```plaintext
Dataset/
├── train/
│   ├── images/
│   └── gt/
├── test/
│   ├── images/
│   └── gt/
└── val/ (optional)


What This Does:
1️⃣ Verifies that the folder structure exists.
2️⃣ Loads images and ground-truth masks.
3️⃣ Resizes all files to 513×513 pixels.
4️⃣ Renames them as 0.jpg → 0.png, 1.jpg → 1.png, etc.
5️⃣ Saves processed outputs into the following structure:

train/src/
train/gt_processed/
test/src/
test/gt_processed/
"""
