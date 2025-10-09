## 🔍 Overview
This folder contains the implementation and benchmarking results of **YOLOv8** for wildfire and smoke detection. YOLOv8 was integrated via the official **Ultralytics PyTorch** framework, which provides pretrained detectors trained on **COCO** and straightforward APIs for **fine-tuning**. The model is evaluated on multiple wildfire datasets to detect **fire** and **smoke regions** in RGB imagery. Performance metrics include **mAP@0.5**, **Precision**, **Recall**, and **F1-score**, along with **cross-dataset generalization** across unseen environments.


## ⚙️ Setup & Requirements
1. **Install dependencies**
   ```bash
   pip install torch torchvision torchaudio scikit-learn tqdm seaborn pillow matplotlib opencv-python
   !pip install ultralytics --quiet
   
git clone https://github.com/<your_repo_name>.git

cd "<your_repo_name>/02 Segmentation -- DeepLab-V3"



## 🧩 Data Organization and Preprocessing
Before running the training scripts, please organize your dataset as follows:

```plaintext
Dataset/
├── train/
│   ├── src/
│   └── gt/
├── test/
│   ├── src/
│   └── gt/
└── val/
    ├── src/
    └── gt/
```

What This Does:\
1️⃣ Verifies that the folder structure exists.\
2️⃣ Loads images and ground-truth masks.\
3️⃣ Resizes all files to 513×513 pixels.\
4️⃣ Renames them as 1.jpg → 1.png, 2.jpg → 2.png, etc.\
5️⃣ Saves processed outputs into the following structure:\

```plaintext
train/src_generated/
train/gt_generated/
test/src_generated/
test/gt_generated/
val/src_generated/
val/gt_generated/
```

## 🧪 Automated Testing on Multiple Datasets

After training, you can automatically evaluate the saved model on the **test subset** of any dataset listed in the repository.  
Simply toggle which datasets to include by setting `True` or `False` in the configuration dictionary, for example:

```python
test_datasets = {
    "WildFireCan": True,
    "Fire360": True,
    "DeepFire": False,
    "FLAME3": True
}
