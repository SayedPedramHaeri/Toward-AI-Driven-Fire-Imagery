## 🔍 Overview
This folder contains the implementation and benchmarking results of **ResNet-50** for wildfire image classification. ResNet-50, a deep residual convolutional neural network, is used to distinguish between **fire** and **non-fire** scenes across multiple wildfire datasets. The model is implemented using the official **torchvision.models** library in PyTorch with pretrained ImageNet weights.  

---

## ⚙️ Setup & Requirements
1. **Install dependencies**
   ```bash
   pip install torch torchvision torchaudio scikit-learn tqdm seaborn pillow matplotlib


git clone https://github.com/<your_repo_name>.git

cd "<your_repo_name>/01 Classification -- ResNet-50"


Dataset/

├── Fire/

│   ├── fire/          # fire images

│   ├── no_Fire/       # non-fire images

