# 🔥 AI-Driven Fire Imagery: The Promise of VLMs and LLMs

A comprehensive repository accompanying the paper **_Toward AI-Driven Fire Imagery: Attributes, Challenges, Comparisons, and the Promise of VLMs and LLMs_ (2025)**. This repository provides code, datasets, and analyses supporting our large-scale review of wildfire and smoke imagery resources, and their integration with both traditional **Computer Vision (CV)** and modern **Vision-Language Models (VLMs)** and **Large Language Models (LLMs)**. It is intended for researchers, practitioners, and students interested in dataset benchmarking, computer-vision-based wildfire management, and multimodal perception.

---

## 🔍 Overview  

Despite substantial advancements in technology-driven fire management systems, the global rise in wildfire frequency and intensity amplified by climate change underscores the urgent need for intelligent, data-driven monitoring frameworks. This repository presents a structured overview of wildfire datasets developed over the past two decades, encompassing **RGB, thermal, infrared, acoustic, chemical, and multimodal** sources. It analyzes their design, annotation standards, and suitability for modern AI applications in detection, prediction, and suppression. Beyond organizing existing resources, it introduces practical guidelines for developing unified, high-quality datasets and highlights how emerging **LLMs** and **VLMs** can advance wildfire research through automated dataset generation, multimodal reasoning, and data-driven decision support for real-time fire management and post-incident assessment.



---

## 📌 What You’ll Find Here  

1. 🔥 **All existing fire and smoke datasets (2005–2025).**  
2. 🧠 **Vision-based classification benchmarks** using ResNet-50.  
3. 🧩 **Vision-based segmentation analysis** using DeepLab-V3.  
4. 🎯 **Vision-based detection experiments** using YOLOv8.  
5. 💡 **Vision-Language classification** with CLIP.  
6. 🌐 **Vision-Language detection** with Grounding-DINO.  


---

## 📚 Structured by Dataset Class  

Instead of algorithm classes, this repository organizes resources **by dataset category**, mirroring *Table 8* of the paper.  
Each entry links to the dataset homepage or download source and specifies modality, task type, and license status.  

### 🔥 Complete Wildfire, Smoke, and Multimodal Dataset Index

| No | Dataset Name | Year | Type | Modality | Tasks | Download Link |
|:--:|:--------------|:----:|:----:|:----------|:------|:--------------|
| 1 | **WildFireCan** | 2025 | Multimodal | Image + Text | Cls / Det | [Download](https://github.com/Multimodal-Social-Media-Data-Analysis/WildfireCanMMD-Multimedia-Classification-on-user-generated-content-During-Wildfires-in-Canada) |
| 2 | **Fire360** | 2025 | Multimodal | RGB + Thermal + Text | Cls / Det | [Download](https://uofi.app.box.com/v/fire360dataset) |
| 3 | **DisasterM3** | 2025 | Multimodal | Satellite + Text (SAR) | Cls / Seg / Det | [Download](https://data.mendeley.com/datasets/zkwgkjkjn9/2) |
| 4 | **FightwithFire** | 2023 | Multimodal | Image + Audio | Cls / Det | N/A |
| 5 | **MultimodalGas** | 2022 | Sensor | Image + Gas | Cls / Det | [Download](https://data.mendeley.com/datasets/zkwgkjkjn9/2) |
| 6 | **FLAME3** | 2024 | Aerial | Multispectral / Thermal | Cls / Det | [Download](https://www.kaggle.com/datasets/brycehopkins/flame-3-computer-vision-subset-sycan-marsh) |
| 7 | **FLAME-SD** | 2024 | Synthetic | RGB | Cls / Det | [Download](https://github.com/AIS-Clemson/FLAME_SD) |
| 8 | **DFS** | 2023 | Aggregated | RGB | Cls / Det | [Download](https://github.com/siyuanwu/DFS-FIRE-SMOKE-Dataset?tab=readme-ov-file) |
| 9 | **BA-UAV** | 2023 | Aerial | UAV Imagery | Seg | [Download](https://github.com/ipleiria-ciic/ees-datalab) |
| 10 | **FireDetn** | 2023 | Image | RGB | Det | [Download](https://github.com/SuperXxts/FireDetn) |
| 11 | **FireFly** | 2023 | Synthetic | RGB | Det | [Download](https://github.com/ERGOWHO/Firefly2.0) |
| 12 | **FLAME2** | 2022 | Aerial | Multispectral / Thermal | Cls | [Download](https://ieee-dataport.org/open-access/flame-2-fire-detection-and-modeling-aerial-multi-spectral-image-dataset) |
| 13 | **FireFront** | 2022 | Simulation | RGB | Cls | N/A |
| 14 | **DeepFire** | 2022 | Image | RGB | Cls | [Download](https://www.kaggle.com/datasets/alik05/forest-fire-dataset) |
| 15 | **Paddle Fire** | 2021 | Image | RGB | Cls | [Download](https://aistudio.baidu.com/datasetdetail/107770) |
| 16 | **DataCluster** | 2021 | Image | RGB | Cls / Det | [Download](https://www.kaggle.com/datasets/dataclusterlabs/fire-and-smoke-dataset) |
| 17 | **WildfireDet** | 2021 | Image | RGB | Cls | [Download](https://www.kaggle.com/datasets/brsdincer/wildfire-detection-image-data) |
| 18 | **FD-Dataset** | 2020 | Image | RGB | Det | N/A |
| 19 | **D-Fire** | 2020 | Mixed | RGB | Cls / Det | [Download](https://github.com/gaiasd/DFireDataset) |
| 20 | **FLAME1** | 2020 | Aerial | Multispectral / Thermal | Cls / Seg | [Download](https://ieee-dataport.org/open-access/flame-dataset-aerial-imagery-pile-burn-detection-using-drones-uavs) |
| 21 | **FF-Det** | 2020 | Image | RGB | Cls | [Download](https://data.mendeley.com/datasets/gjmr63rz2r/1) |
| 22 | **FireNet** | 2019 | Image | RGB | Det | [Download](https://github.com/OlafenwaMoses/FireNet) |
| 23 | **AIDER** | 2019 | Aerial | RGB | Cls | [Download](https://github.com/ckyrkou/AIDER) |
| 24 | **ForestryImage** | 2018 | Image | RGB | Cls | [Download](https://www.forestryimages.org/browse/subthumb.cfm?sub=740) |
| 25 | **FIRE** | 2018 | Image | RGB | Cls | [Download](https://www.kaggle.com/datasets/phylake1337/fire-dataset) |
| 26 | **CAIR** | 2017 | Image | RGB | Cls | [Download](https://github.com/cair/Fire-Detection-Image-Dataset) |
| 27 | **FESB MLID** | 2017 | Image | RGB | Cls / Seg | [Download](http://wildfire.fesb.hr/) |
| 28 | **FiSmo** | 2017 | Video | RGB | Cls | [Download](https://github.com/mtcazzolato/dsw2017) |
| 29 | **Corsican** | 2017 | Image | RGB | Seg | [Download](https://cfdb.univ-corse.fr/index.php) |
| 30 | **FireSense** | 2017 | Video | RGB | Cls | [Download](https://zenodo.org/records/836749) |
| 31 | **BoWFire** | 2015 | Image | RGB | Cls / Seg | [Download](https://bitbucket.org/gbdi/bowfire-dataset/downloads/) |
| 32 | **MIVIA** | 2014 | Video | RGB | Cls | [Download](https://mivia.unisa.it/datasets/video-analysis-datasets/fire-detection-dataset/) |
| 33 | **VisiFire** | 2010 | Video | RGB | Cls | [Download](http://signal.ee.bilkent.edu.tr/VisiFire/) |
| 34 | **FireClips** | 2006 | Video | RGB | Cls | [Download](http://signal.ee.bilkent.edu.tr/VisiFire/Demo/FireClips/) |
| 35 | **ForestFireSound** | 2024 | Acoustic | Audio | Cls | N/A |
| 36 | **ForestSound** | 2023 | Acoustic | Audio | Cls / Det | N/A |
| 37 | **FSC22** | 2023 | Acoustic | Audio | Cls | [Download](https://ieee-dataport.org/documents/fsc22-dataset) |
| 38 | **FireSound** | 2021 | Acoustic | Audio | Cls / Det | [Download](https://www.kaggle.com/datasets/forestprotection/forest-wild-fire-sound-dataset) |
| 39 | **IberFire** | 2025 | Meteorological | Spatio-Temporal | Cls | [Download](https://zenodo.org/records/1522588) |
| 40 | **Algerian** | 2019 | Meteorological | Spatio-Temporal | Cls | [Download](https://archive.ics.uci.edu/dataset/547/algerian+forest+fires+dataset) |
| 41 | **SmokeDet** | 2022 | Chemical | Gas Sensors | Cls | [Download](https://www.kaggle.com/datasets/deepcontractor/smoke-detection-dataset) |
| 42 | **EarlyFire** | 2022 | Chemical | Gas Sensors | Cls / Det | [Download](https://data.mendeley.com/datasets/f3mjnbm9b3/1) |

---

**Legend**  
- **Cls** = Classification | **Seg** = Segmentation | **Det** = Detection  
- **Multimodal** datasets combine two or more data types (e.g., image + audio or image + text).  
- **Aerial / UAV** datasets are captured via drones or satellites.  
- **Synthetic / Aggregated** datasets are artificially generated or compiled from multiple sources.  



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
---

## 📄 License  

This project is open-source under the [MIT License](LICENSE).  

If you use this repository, please cite:  

> S. P. Haeri Boroujeni *et al.*,  
> “Toward AI-Driven Fire Imagery: Attributes, Challenges, Comparisons, and the Promise of VLMs and LLMs,” 2025.  

---

