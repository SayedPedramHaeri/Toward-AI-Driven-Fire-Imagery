# Toward AI-Driven Fire Imagery: Attributes, Challenges, Comparisons, and the Promise of VLMs and LLMs  

A comprehensive repository accompanying the paper **_Toward AI-Driven Fire Imagery: Attributes, Challenges, Comparisons, and the Promise of VLMs and LLMs_ (2025)**. This repository provides code, datasets, and analyses supporting our large-scale review of wildfire and smoke imagery resources and their integration with modern **Vision-Language Models (VLMs)** and **Large Language Models (LLMs)**. It is intended for researchers, practitioners, and students interested in **dataset benchmarking**, **computer-vision-based wildfire management**, and **multimodal perception**.

---

## 🔍 Overview  

Despite major advances in technology-driven fire-management systems, global wildfire frequency and severity continue to rise—exacerbated by climate change and limited resource allocation.  
This work addresses the need for intelligent, data-driven fire-monitoring frameworks powered by AI and **Unmanned Aerial Systems (UAS)**.  

We review, organize, and compare all significant wildfire datasets released over the last 20 years (**RGB, thermal, IR, acoustic, chemical, multimodal**), analyzing their structure, annotation, and usability for modern AI tasks.  
The study also explores how emerging **LLMs and VLMs** can accelerate the **creation, augmentation, and application** of fire datasets for early detection, spread prediction, and post-incident assessment.

---

## 📌 What You’ll Find Here  

1. 🔥 **All existing fire and smoke datasets (2005–2025)** — curated and categorized by sensor type, modality, and application.  
2. 🧠 **Vision-based classification benchmarks** using ResNet-50 on standard RGB datasets.  
3. 🧩 **Vision-based segmentation analysis** using DeepLab-V3 for pixel-level smoke and flame mapping.  
4. 🎯 **Vision-based detection experiments** using YOLOv8 on aerial and ground-view datasets.  
5. 💡 **Vision-Language classification** with CLIP for multimodal understanding and zero-shot recognition.  
6. 🌐 **Vision-Language detection** with Grounding-DINO for open-vocabulary fire and smoke localization.  

Each implementation includes evaluation scripts, pretrained checkpoints (when available), and cross-dataset benchmarking utilities.

---

## 📚 Structured by Dataset Class  

Instead of algorithm classes, this repository organizes resources **by dataset category**, mirroring *Table 8* of the paper.  
Each entry links to the dataset homepage or download source and specifies modality, task type, and license status.  

| No | Dataset Name | Year | Type | Modality | Tasks | Download Link |
|:--:|:--------------|:----:|:----:|:----------|:------|:--------------|
| 1 | **WildFireCan** | 2025 | Multimodal | Image + Text | Cls / Det | [Download](https://github.com/Multimodal-Social-Media-Data-Analysis/WildfireCanMMD-Multimedia-Classification-on-user-generated-content-During-Wildfires-in-Canada) |
| 2 | **Fire360** | 2025 | Video + Text | VQA + Reasoning | Cls / Seg / Det | [Download](https://uofi.app.box.com/v/fire360dataset) |
| 3 | **DisasterM3** | 2025 | Satellite + Text | SAR + Captions | Cls / Seg / Det | [Download](https://data.mendeley.com/datasets/zkwgkjkjn9/2) |
| 4 | **FLAME Series (1–3)** | 2020–2024 | Aerial | Multispectral / Thermal | Cls / Det | Available upon request |
| 5 | **DeepFire** | 2022 | Image | RGB | Cls | [Download](https://data.mendeley.com/datasets/6x4cgwhd7z/1) |
| 6 | **FireDetn** | 2023 | Image | RGB | Det | N/A |
| 7 | **BA-UAV** | 2023 | Video | Aerial | Seg | N/A |
| 8 | **FightwithFire** | 2023 | Image + Audio | Multimodal | Cls / Det | N/A |
| 9 | **MultimodalGas** | 2022 | Image + Gas | Sensor Fusion | Cls | N/A |
| 10 | **SmokeDet / EarlyFire** | 2022 | Chemical | Gas Sensors | Cls / Det | N/A |
| ... | *Full dataset list continues in paper Table 8* |  |  |  |  |  |

---

## 🧪 Experiments  

### Vision Benchmarks  
- Implementations of **ResNet-50**, **DeepLab-V3**, and **YOLOv8** in PyTorch.  
- Benchmarked on multiple wildfire datasets for **classification**, **segmentation**, and **object detection**.  

### Vision–Language Benchmarks  
- **CLIP** for multimodal fire classification and zero-shot recognition.  
- **Grounding-DINO** for open-vocabulary wildfire detection.  

### Evaluation Metrics  
- Accuracy, IoU, mAP@50, F1-Score, Precision/Recall  
- Cross-dataset generalization indices  

Each experiment includes a Jupyter notebook detailing dataset loading, training, and evaluation workflows.

---

## 📊 Visualizations  

- Dataset distribution plots (fire vs. non-fire ratios, modality coverage, geographic balance)  
- Model performance curves and confusion matrices  
- Qualitative segmentation and detection samples  

---

## 🧑‍💻 Authors  

**Sayed Pedram Haeri Boroujeni**  
PhD Student, Clemson University  
📧 [sayedpedramhaeri@gmail.com](mailto:sayedpedramhaeri@gmail.com)  

**Niloufar Mehrabi**, **Fatemeh Afghah**, **Connor McGrath**, **Danish Bhatkar**, **Mithilesh Biradar**, **Abolfazl Razi**  

---

## 📄 License  

This project is open-source under the [MIT License](LICENSE).  

If you use this repository, please cite:  

> S. P. Haeri Boroujeni *et al.*,  
> “Toward AI-Driven Fire Imagery: Attributes, Challenges, Comparisons, and the Promise of VLMs and LLMs,” 2025.  

---

## ⭐ Acknowledgments  

This work was supported by the **National Aeronautics and Space Administration (NASA)** under Award No. 80NSSC23K1393, and by the **National Science Foundation (NSF)** under Grant Nos. CNS-2232048, CNS-2120485, and CNS-2204445.  

---
