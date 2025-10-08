## 🔍 Overview
This folder contains the implementation and benchmarking results of **ResNet-50** for wildfire image classification. ResNet-50, a deep residual convolutional neural network, is used to distinguish between **fire** and **non-fire** scenes across multiple wildfire datasets. The model is implemented using the official **torchvision.models** library in PyTorch with pretrained ImageNet weights.  

---

## ⚙️ Setup & Requirements
1. **Install dependencies**
   ```bash
   pip install torch torchvision torchaudio scikit-learn tqdm seaborn pillow matplotlib


git clone https://github.com/<your_repo_name>.git

cd "<your_repo_name>/01 Classification -- ResNet-50"


## 🧩 Data Preprocessing

When you run the notebook, the dataset is automatically preprocessed and split into:

- **Training (60 %)**
- **Validation (20 %)**
- **Testing (20 %)**

If these folders already exist, the code detects them automatically and skips re-splitting.  
All images are resized to **224 × 224 px** to match the ResNet-50 input requirements.  
Each image file is renamed sequentially within its subset (e.g., `1.jpg`, `2.jpg`, …).  
Class balance and the number of samples per subset are printed at the end of preprocessing, allowing users to verify the integrity of the dataset.

The preprocessing pipeline performs:
1. Automatic detection of class folders (e.g., `Fire/`, `no_Fire/`).
2. Randomized data splitting using a fixed seed for reproducibility.
3. Image resizing, conversion to RGB, and sequential renaming.
4. Summary statistics showing counts for each class and split.
