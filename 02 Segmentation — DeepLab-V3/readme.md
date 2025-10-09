## 🔍 Overview
This directory includes experiments based on **DeepLab-V3**, a state-of-the-art semantic segmentation model used for **pixel-level fire and smoke delineation**. The model leverages atrous spatial pyramid pooling (ASPP) to capture multi-scale contextual information. All implementations utilize **torchvision.models.segmentation** with pretrained COCO weights.


## ⚙️ Setup & Requirements
1. **Install dependencies**
   ```bash
   pip install torch torchvision torchaudio scikit-learn tqdm seaborn pillow matplotlib opencv-python

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
