# 🌙 Awesome Low-Light Video Datasets

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

A curated collection of datasets for **Low-Light Image Enhancement (LLIE)** and **Low-Light Video Enhancement (LLVE)** research.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Datasets](#-datasets)
  - [SDSD Dataset](#1-sdsd-dataset)
  - [Nankai LLIE Collection](#2-nankai-llie-collection)
  - [BVI-LowLight Dataset](#3-bvi-lowlight-dataset)
  - [EvLight Dataset](#4-evlight-dataset)
  - [LLIE Survey Dataset](#5-llie-survey-dataset)
  - [Seeing Motion in the Dark](#6-seeing-motion-in-the-dark-smitd)
  - [SMID Dataset](#7-smid-dataset)
  - [DID Dataset](#8-did-dataset)
- [Quick Comparison](#-quick-comparison)
- [Citation](#-citation)
- [Contributing](#-contributing)

---

## 📖 Overview

Low-light image and video enhancement is a fundamental task in computer vision. This repository provides a comprehensive collection of publicly available datasets for training and evaluating low-light enhancement algorithms.

**Key Challenges in Low-Light Imaging:**
- Reduced illumination intensity and increased photon noise
- Trade-offs between aperture, shutter speed, and ISO settings
- Color distortion and white balance issues
- Motion blur in dynamic scenes
- Adverse effects on downstream tasks (detection, classification)

---

## 📦 Datasets

### 1. SDSD Dataset

**Static and Dynamic Scenes Dataset**

| Property | Details |
|----------|---------|
| **Type** | Video Pairs (Low-light / Normal-light) |
| **Indoor Subset** | 70 video pairs |
| **Outdoor Subset** | 80 video pairs |
| **Total** | 150 video pairs |
| **Format** | Dynamic video sequences |

**Description:**  
The SDSD dataset is collected in the form of dynamic video pairs, containing both low-light and normal-light videos. It consists of two subsets: an indoor subset with 70 video pairs and an outdoor subset with 80 video pairs, making it ideal for evaluating video enhancement methods in diverse environments.

🔗 **Link:** [SDSD Dataset](https://github.com/JIA-Lab-research/SDSD)

---

### 2. Nankai LLIE Collection

**Lighting the Darkness in the Deep Learning Era**

| Property | Details |
|----------|---------|
| **Type** | Images & Videos |
| **Source** | Various smartphone cameras |
| **Conditions** | Multiple lighting conditions |
| **Scenes** | Diverse real-world scenarios |

**Description:**  
A comprehensive collection from Professor Chongyi Li's research group at Nankai University. This dataset includes images and videos captured by various smartphone cameras under different lighting conditions and scenes, providing realistic low-light scenarios for algorithm evaluation.

🔗 **Link:** [Nankai LLIE Collection](https://github.com/Li-Chongyi/Lighting-the-Darkness-in-the-Deep-Learning-Era-Open)

---

### 3. BVI-LowLight Dataset

**Fully Registered Dataset for Low-Light Enhancement**

| Property | Details |
|----------|---------|
| **Type** | Images & Videos (Fully Registered) |
| **Features** | Multiple exposure settings |
| **Alignment** | Pixel-level registration |
| **Application** | Enhancement & Machine Learning |

**Description:**  
Images and videos captured under low-light conditions often suffer from distortions due to the interplay of aperture, shutter speed, and ISO settings. These interactions lead to image degradation, particularly under extreme lighting conditions. The distortion primarily arises from the inverse relationship between reduced illumination intensity and increased photon noise, which becomes more pronounced with higher sensor gain. Additionally, white balance and color rendition are adversely affected, potentially requiring post-processing corrections.

These distortions not only impact perceptual image quality but also pose significant challenges for machine learning tasks, including classification and object detection—especially considering the sensitivity of deep learning networks to adversarial samples.

🔗 **Link:** [BVI-LowLight Dataset](https://ieee-dataport.org/open-access/bvi-lowlight-fully-registered-datasets-low-light-image-and-video-enhancement)

---

### 4. EvLight Dataset

**Event-based Low-Light Enhancement Dataset**

| Property | Details |
|----------|---------|
| **Type** | Aligned Low-light Data |
| **Features** | Event camera + RGB alignment |
| **Application** | Event-guided enhancement |

**Description:**  
EvLight provides aligned low-light data specifically designed for event-guided low-light video enhancement. The dataset leverages event cameras' high dynamic range capabilities for improved low-light reconstruction.

🔗 **Link:** [EvLight Dataset](https://github.com/EthanLiang99/EvLight)

---

### 5. LLIE Survey Dataset

**Aerial & Street View Collection**

| Property | Details |
|----------|---------|
| **Type** | Images |
| **Scenes** | Aerial + Street View |
| **Size** | ~26 GB |
| **Coverage** | Large-scale diverse scenarios |

**Description:**  
A large-scale dataset accompanying the LLIE survey paper, featuring aerial photography and street view images. With approximately 26GB of data, it provides extensive coverage for training robust low-light enhancement models.

🔗 **Link:** [LLIE Survey Dataset](https://github.com/ShenZheng2000/LLIE_Survey)

---

### 6. Seeing Motion in the Dark (SMITD)

**Extreme Low-Light Video Dataset**

| Property | Details |
|----------|---------|
| **Type** | RAW Video Pairs |
| **Features** | Short-exposure / Long-exposure pairs |
| **Conditions** | Extreme darkness |
| **Format** | RAW sensor data |

**Description:**  
This dataset focuses on extreme low-light conditions with paired short-exposure and long-exposure video sequences. It enables research on RAW video enhancement and motion-aware processing in challenging lighting scenarios.

🔗 **Link:** [Seeing Motion in the Dark](https://github.com/cchen156/Seeing-Motion-in-the-Dark)

---

### 7. SMID Dataset

**See Moving objects in the Dark**

| Property | Details |
|----------|---------|
| **Type** | Video Sequences |
| **Features** | Moving objects in low-light |
| **Storage** | Baidu Pan |

**Description:**  
The SMID dataset complements the SDSD dataset, focusing on capturing moving objects under low-light conditions.

🔗 **Link:** [SMID Dataset (Baidu Pan)](https://pan.baidu.com/s/1Qol_4GsIjGDR8UT9IRZbBQ#list/path=%2F)  
🔑 **Password:** `btux`

📂 **Source Repository:** [JIA-Lab SDSD](https://github.com/JIA-Lab-research/SDSD)

---

### 8. DID Dataset

**Dark Image/Video Dataset (ICCV 2023)**

| Property | Details |
|----------|---------|
| **Type** | Images & Videos |
| **Publication** | ICCV 2023 |
| **Purpose** | General Low-light Video Enhancement Benchmark |

**Description:**  
DID serves as a benchmark towards general low-light video enhancement, introduced at ICCV 2023. It provides standardized evaluation protocols for comparing video enhancement methods.

📄 **Paper:** *A Benchmark towards General Low-light Video Enhancement* (ICCV 2023)

🔗 **Link:** [DID Dataset](https://github.com/ciki000/DID)

---

## 📊 Quick Comparison

| Dataset | Type | Paired | Video | Size | Special Features |
|---------|------|--------|-------|------|------------------|
| SDSD | Video | ✅ | ✅ | 150 pairs | Indoor/Outdoor subsets |
| Nankai LLIE | Image+Video | ✅ | ✅ | - | Multi-device capture |
| BVI-LowLight | Image+Video | ✅ | ✅ | - | Fully registered |
| EvLight | Video | ✅ | ✅ | - | Event camera aligned |
| LLIE Survey | Image | ✅ | ❌ | 26GB | Aerial + Street view |
| SMITD | RAW Video | ✅ | ✅ | - | Extreme darkness |
| SMID | Video | ✅ | ✅ | - | Moving objects |
| DID | Image+Video | ✅ | ✅ | - | ICCV 2023 benchmark |

---

## 📚 Citation

If you find this collection useful, please consider citing the original dataset papers:

```bibtex
@inproceedings{wang2021sdsd,
  title={Seeing Dynamic Scene in the Dark: A High-Quality Video Dataset with Mechatronic Alignment},
  author={Wang, Ruixing and others},
  booktitle={ICCV},
  year={2021}
}

@article{li2021low,
  title={Low-Light Image and Video Enhancement Using Deep Learning: A Survey},
  author={Li, Chongyi and others},
  journal={IEEE TPAMI},
  year={2021}
}

@inproceedings{chen2019seeing,
  title={Seeing Motion in the Dark},
  author={Chen, Chen and others},
  booktitle={ICCV},
  year={2019}
}

@inproceedings{fu2023did,
  title={Dancing in the Dark: A Benchmark towards General Low-light Video Enhancement},
  author={Fu, Xiaogang and others},
  booktitle={ICCV},
  year={2023}
}
```

---

## 🤝 Contributing

Contributions are welcome! If you know of any other low-light datasets that should be included:

1. Fork this repository
2. Add the dataset information following the existing format
3. Submit a pull request

---

## 📄 License

This repository is licensed under the MIT License. Please refer to individual dataset licenses for usage terms.

---

## ⭐ Acknowledgements

We thank all the researchers who have made their datasets publicly available to advance low-light enhancement research.

---

<p align="center">
  <i>If you find this collection helpful, please consider giving it a ⭐!</i>
</p>
