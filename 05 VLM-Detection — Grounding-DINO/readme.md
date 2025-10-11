## 🔍 Overview
This folder includes the **Grounding-DINO** implementation for **open-vocabulary object detection** of fire and smoke phenomena.  
Grounding-DINO integrates vision and language modalities to perform **natural-language–driven detection**, enabling flexible prompts such as “find smoke in the image.”  
Experiments are based on the official **IDEA-Research** PyTorch repository using pretrained checkpoints. Evaluation focuses on localization accuracy, detection recall, and generalization to unseen wildfire scenes.


## ⚙️ Setup & Requirements
1. **Install dependencies**
   ```bash
   pip install torch torchvision torchaudio scikit-learn tqdm seaborn pillow matplotlib
   git clone https://github.com/IDEA-Research/GroundingDINO.git
   cd GroundingDINO
   
git clone https://github.com/<your_repo_name>.git

cd "<your_repo_name>/01 Classification -- CLIP"


## 🧩 Data Organization and Preprocessing
Before running the testing scripts, please organize your dataset as follows:

```plaintext
Dataset/
├── train/
│   ├── fire/
│   └── no_fire/
├── test/
│   ├── fire/
│   └── no_fire/
└── val/
    ├── fire/
    └── no_fire/
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

