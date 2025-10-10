## 🔍 Overview
This folder contains the implementation and benchmarking results of **ResNet-50** for wildfire image classification. ResNet-50, a deep residual convolutional neural network, is used to distinguish between **fire** and **non-fire** scenes across multiple wildfire datasets. The model is implemented using the official **torchvision.models** library in PyTorch with pretrained ImageNet weights.  

---

## ⚙️ Setup & Requirements
1. **Install dependencies**
   ```bash
   pip install torch torchvision torchaudio scikit-learn tqdm seaborn pillow matplotlib
   
git clone https://github.com/<your_repo_name>.git

cd "<your_repo_name>/01 Classification -- ResNet-50"


## 🧩 Data Organization and Preprocessing
Before running the training scripts, please organize your dataset as follows:

```plaintext
Dataset/
├── train/
│   ├── Fire/
│   └── No_Fire/
├── test/
│   ├── Fire/
│   └── No_Fire/
└── val/
    ├── Fire/
    └── No_Fire/
```

What This Does:\
1️⃣ Verifies that the folder structure exists.\
2️⃣ The code detects them automatically and skips re-splitting.\
3️⃣ Resizes all files to 224×224 pixels.\
4️⃣ Renames them as 1.jpg → 1.png, 2.jpg → 2.png, etc.\
5️⃣ Saves processed outputs into the following structure:\

---

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


