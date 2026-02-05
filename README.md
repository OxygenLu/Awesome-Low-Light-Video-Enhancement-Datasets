# 🌙 Awesome Low-Light Video Enhancement Datasets

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
![Last Update](https://img.shields.io/badge/Last%20Update-2025-blue)

A curated collection of datasets for **Low-Light Image Enhancement (LLIE)** and **Low-Light Video Enhancement (LLVE)** research.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Datasets](#-datasets)
  - [Video Datasets](#video-datasets)
  - [Image Datasets](#image-datasets)
  - [Challenge Datasets](#challenge-datasets)
- [Recent Methods (2024-2025)](#-recent-methods-2024-2025)
- [Quick Comparison](#-quick-comparison)
- [Related Resources](#-related-resources)
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

### Video Datasets

#### 1. SDSD Dataset

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

#### 2. Nankai LLIE Collection

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

#### 3. BVI-LowLight / BVI-RLV Dataset 🆕

**Fully Registered Dataset for Low-Light Video Enhancement (2024)**

| Property | Details |
|----------|---------|
| **Type** | Videos (Fully Registered) |
| **Scenes** | 40 scenes |
| **Conditions** | Two distinct low-lighting conditions |
| **Features** | Genuine noise and temporal artifacts |
| **Alignment** | Pixel-level registration via motorized dolly |
| **Publication** | arXiv 2024 |

**Description:**  
Low-light videos often exhibit spatiotemporal incoherent noise, leading to poor visibility and compromised performance across various computer vision applications. This paper introduces a novel low-light video dataset, consisting of 40 scenes captured in various motion scenarios under two distinct low-lighting conditions, incorporating genuine noise and temporal artifacts. Fully registered ground truth data is captured in normal light using a programmable motorized dolly. Benchmarks using CNNs, Transformers, Diffusion models, and **Mamba (State Space Models)** are provided.

📄 **Paper:** [BVI-RLV: A Fully Registered Dataset and Benchmarks for Low-Light Video Enhancement](https://arxiv.org/abs/2407.03535) (July 2024)

🔗 **Link:** [IEEE DataPort](https://ieee-dataport.org/open-access/bvi-lowlight-fully-registered-datasets-low-light-image-and-video-enhancement)

---

#### 4. EvLight Dataset

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

#### 5. Night Wenzhou Dataset 🆕

**Large-Scale Aerial & Street View Video Dataset (2024)**

| Property | Details |
|----------|---------|
| **Type** | High-resolution Videos |
| **Scenes** | Aerial + Street View |
| **Size** | ~26 GB |
| **Duration** | 2 hours 3 minutes |
| **Equipment** | DJI Mini 2 (aerial), GoPro HERO7 (street) |
| **FPS** | 30 |

**Description:**  
Night Wenzhou is a large-scale, high-resolution video dataset captured during fast motions with diverse illuminations (extremely dark, underexposure, moonlight, uneven illumination), various landscapes, and miscellaneous degradation (noise, blur, shadows, artifacts). It facilitates the application of LLIE methods to real-world challenges like autonomous driving and UAV.

📄 **Paper:** [Low-Light Image and Video Enhancement: A Comprehensive Survey and Beyond](https://arxiv.org/abs/2212.10772) (Updated 2024)

🔗 **Link:** [LLIE Survey Dataset](https://github.com/ShenZheng2000/LLIE_Survey)

---

#### 6. Seeing Motion in the Dark (SMITD)

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

#### 7. SMID Dataset

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

#### 8. DID Dataset

**Dark Image/Video Dataset (ICCV 2023)**

| Property | Details |
|----------|---------|
| **Type** | Images & Videos |
| **Publication** | ICCV 2023 |
| **Purpose** | General Low-light Video Enhancement Benchmark |

**Description:**  
DID serves as a benchmark towards general low-light video enhancement, introduced at ICCV 2023. It provides standardized evaluation protocols for comparing video enhancement methods.

📄 **Paper:** *Dancing in the Dark: A Benchmark towards General Low-light Video Enhancement* (ICCV 2023)

🔗 **Link:** [DID Dataset](https://github.com/ciki000/DID)

---

### Image Datasets

#### 9. VE-LOL Dataset

**Vision Enhancement in the LOw-Light condition**

| Property | Details |
|----------|---------|
| **Type** | Large-scale Images |
| **Total Images** | 13,440 |
| **VE-LOL-L (Paired)** | 2,100 training + 400 testing pairs |
| **VE-LOL-H (Unpaired)** | 6,940 training + 4,000 testing |
| **Features** | Face detection annotations |
| **Scenes** | Natural landscapes, urban streets, human faces |

**Description:**  
VE-LOL is a large-scale dataset covering diverse scenes. It comprises two subsets: VE-LOL-L (paired) and VE-LOL-H (unpaired with face detection bounding box annotations), enabling joint low-light enhancement and detection benchmarking.

🔗 **Link:** [VE-LOL Benchmark](https://flyywh.github.io/IJCV2021LowLight_VELOL/)

---

#### 10. UHD-LOL Dataset 🆕

**Ultra-High-Definition Low-Light Dataset (AAAI 2023)**

| Property | Details |
|----------|---------|
| **UHD-LOL4K** | 8,099 pairs (5,999 train / 2,100 test) |
| **UHD-LOL8K** | 2,966 pairs (2,029 train / 937 test) |
| **Resolution** | 4K and 8K |
| **Scenes** | Indoor/outdoor, buildings, streets, people |

**Description:**  
The first large-scale UHD low-light image enhancement dataset, designed to benchmark the performance of existing LLIE methods on ultra-high-definition images. Includes both 4K and 8K resolution subsets.

📄 **Paper:** *Ultra-High-Definition Low-Light Image Enhancement: A Benchmark and Transformer-Based Method* (AAAI 2023)

🔗 **Link:** [LLFormer / UHD-LOL](https://github.com/TaoWangzj/LLFormer)

---

#### 11. LOL-Blur Dataset 🆕

**Joint Low-Light Enhancement and Deblurring (ECCV 2022)**

| Property | Details |
|----------|---------|
| **LOL-Blur** | 12,000 pairs (170 videos train / 30 videos test) |
| **Real-LOL-Blur** | 1,354 real-world night blurry images |
| **Features** | Low-blur/normal-sharp pairs |
| **Task** | Joint enhancement and deblurring |

**Description:**  
The first large-scale dataset for joint low-light enhancement and deblurring. Contains diverse darkness and motion blurs, with realistic blur simulation including saturated regions (light streaks). Real-LOL-Blur includes 482 images from RealBlur-J and 872 images captured by Sony RX10 IV.

📄 **Paper:** *LEDNet: Joint Low-light Enhancement and Deblurring in the Dark* (ECCV 2022)

🔗 **Link:** [LEDNet / LOL-Blur](https://github.com/sczhou/LEDNet)  
📥 **Download:** [Google Drive](https://drive.google.com/drive/folders/1bRBG8DG_72AGA6-eRePvChlT5ZO4cwJ4) / [Baidu Pan](https://pan.baidu.com/s/1-M0IIewjdgXFP2vC2R6_7A) (key: dz6u)

---

#### 12. SICE_Grad & SICE_Mix 🆕

**Mixed Over-/Under-Exposure Datasets (2024)**

| Property | Details |
|----------|---------|
| **Type** | Images with mixed exposure |
| **Feature** | Both over- and under-exposure in single images |
| **Base** | Extended from SICE dataset |

**Description:**  
The first datasets that include both overexposure and underexposure in single images, addressing a previously unresolved challenge in the LLIE community.

🔗 **Link:** [LLIE Survey Dataset](https://github.com/ShenZheng2000/LLIE_Survey)

---

### Challenge Datasets

#### 13. NTIRE 2024 LLIE Dataset 🆕

**CVPR NTIRE 2024 Challenge Dataset**

| Property | Details |
|----------|---------|
| **Type** | High-resolution Images |
| **Resolution** | Up to 4K and beyond |
| **Conditions** | Non-uniform illumination, backlighting, extreme darkness, night scenes |
| **Participants** | 428 registered, 22 valid submissions |

**Description:**  
A new LLIE dataset built for the NTIRE 2024 Challenge, featuring a wide range of scenes with various low-light conditions including indoor/outdoor, daytime/nighttime scenarios. Addresses limitations of existing datasets (limited scene diversity, low resolution, overly simplistic lighting).

📄 **Paper:** [NTIRE 2024 Challenge on Low Light Image Enhancement: Methods and Results](https://arxiv.org/abs/2404.14248)

🔗 **Challenge:** [NTIRE 2024](https://cvlai.net/ntire/2024/)

---

#### 14. NTIRE 2025 LLIE Dataset 🆕

**CVPR NTIRE 2025 Challenge Dataset**

| Property | Details |
|----------|---------|
| **Type** | High-resolution Images |
| **Resolution** | 2000×2992 to 4000×6000 |
| **Winner** | FusionNet (HVI-CIDNet + Retinexformer + ESDNet) |

**Description:**  
The latest challenge dataset for low-light image enhancement, continuing to push the boundaries of LLIE research with even more challenging scenarios.

📄 **Paper:** [NTIRE 2025 Challenge on Low Light Image Enhancement: Methods and Results](https://openaccess.thecvf.com/content/CVPR2025W/NTIRE/papers/Liu_NTIRE_2025_Challenge_on_Low_Light_Image_Enhancement_Methods_and_CVPRW_2025_paper.pdf)

---

## 🔬 Recent Methods (2024-2025)

### State-of-the-Art Methods

| Method | Venue | Key Features | Link |
|--------|-------|--------------|------|
| **HVI-CIDNet** | CVPR 2025 | New HVI color space, NTIRE 2025 Winner | [GitHub](https://github.com/Fediory/HVI-CIDNet) |
| **Retinexformer** | ICCV 2023 / NTIRE 2024 Runner-up | Retinex-based Transformer | [GitHub](https://github.com/caiyuanhao1998/Retinexformer) |
| **LLFormer** | AAAI 2023 | UHD enhancement, axis-based Transformer | [GitHub](https://github.com/TaoWangzj/LLFormer) |
| **LEDNet** | ECCV 2022 | Joint enhancement + deblurring | [GitHub](https://github.com/sczhou/LEDNet) |
| **LIEDNet** | TCSVT 2025 | Lightweight enhancement + deblurring with VMamba | [GitHub](https://github.com/MingyuLiu1/LIEDNet) |

### Mamba-based Methods (2024-2025)

| Method | Key Features | Link |
|--------|--------------|------|
| **MambaLLIE** | Implicit Retinex-Aware, Global-then-Local SSM (NeurIPS 2024) | [Paper](https://arxiv.org/abs/2405.16105) |
| **Wave-Mamba** | Wavelet SSM for UHD enhancement (ACM MM 2024) | [GitHub](https://github.com/AlexZou14/Wave-Mamba) |
| **Retinexmamba** | Retinex-based Mamba | [GitHub](https://github.com/YhuoyuH/Retinexmamba) |
| **LLEMamba** | Relighting-Guided with Deep Unfolding | [Paper](https://arxiv.org/abs/2406.01028) |

### Diffusion-based Methods (2024-2025)

| Method | Key Features | Link |
|--------|--------------|------|
| **Reti-Diff** | Retinex-based Latent Diffusion (ICLR 2025 Spotlight) | [Paper](https://arxiv.org/abs/2311.11638) |
| **DiffLL** | Diffusion-based Low-Light Enhancement | [Paper](https://arxiv.org/abs/2304.09748) |

---

## 📊 Quick Comparison

| Dataset | Type | Year | Paired | Video | Size | Special Features |
|---------|------|------|--------|-------|------|------------------|
| SDSD | Video | 2021 | ✅ | ✅ | 150 pairs | Indoor/Outdoor subsets |
| Nankai LLIE | Image+Video | 2021 | ✅ | ✅ | - | Multi-device capture |
| BVI-RLV | Video | 2024 | ✅ | ✅ | 40 scenes | Fully registered, Mamba benchmarks |
| EvLight | Video | 2023 | ✅ | ✅ | - | Event camera aligned |
| Night Wenzhou | Video | 2024 | ❌ | ✅ | 26GB | Aerial + Street view, UAV |
| SMITD | RAW Video | 2019 | ✅ | ✅ | - | Extreme darkness |
| SMID | Video | 2020 | ✅ | ✅ | - | Moving objects |
| DID | Image+Video | 2023 | ✅ | ✅ | - | ICCV 2023 benchmark |
| VE-LOL | Image | 2021 | ✅/❌ | ❌ | 13,440 | Face detection annotations |
| UHD-LOL | Image | 2023 | ✅ | ❌ | 11,065 pairs | 4K/8K resolution |
| LOL-Blur | Image | 2022 | ✅ | ❌ | 12,000 pairs | Joint deblurring |
| NTIRE 2024 | Image | 2024 | ✅ | ❌ | - | Challenge dataset, 4K+ |
| NTIRE 2025 | Image | 2025 | ✅ | ❌ | - | Latest challenge dataset |

---

## 🔗 Related Resources

### Awesome Lists
- [Awesome Low-Light Image Enhancement](https://github.com/zhihongz/awesome-low-light-image-enhancement) - Comprehensive resource list
- [Awesome Mamba in Low-Level Vision](https://github.com/csguoh/Awesome-Mamba-in-Low-Level-Vision) - Mamba-based methods
- [Awesome Vision Mamba Models](https://github.com/Ruixxxx/Awesome-Vision-Mamba-Models) - Vision Mamba survey

### Surveys
- [Low-Light Image and Video Enhancement: A Comprehensive Survey and Beyond](https://arxiv.org/abs/2212.10772) (2024)
- [Diffusion Models for Low-Light Image Enhancement](https://arxiv.org/abs/2510.05976) (2025)
- [Low-Light Image and Video Enhancement for More Robust Computer Vision Tasks](https://pmc.ncbi.nlm.nih.gov/articles/PMC12027663/) (2025)

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

@article{lin2024bvirlv,
  title={BVI-RLV: A Fully Registered Dataset and Benchmarks for Low-Light Video Enhancement},
  author={Lin, Ruirui and others},
  journal={arXiv preprint arXiv:2407.03535},
  year={2024}
}

@inproceedings{zhou2022lednet,
  title={LEDNet: Joint Low-light Enhancement and Deblurring in the Dark},
  author={Zhou, Shangchen and Li, Chongyi and Loy, Chen Change},
  booktitle={ECCV},
  year={2022}
}

@inproceedings{wang2023llformer,
  title={Ultra-High-Definition Low-Light Image Enhancement: A Benchmark and Transformer-Based Method},
  author={Wang, Tao and others},
  booktitle={AAAI},
  year={2023}
}

@inproceedings{yan2025hvi,
  title={HVI: A New Color Space for Low-light Image Enhancement},
  author={Yan, Qingsen and others},
  booktitle={CVPR},
  year={2025}
}

@inproceedings{cai2023retinexformer,
  title={Retinexformer: One-stage Retinex-based Transformer for Low-light Image Enhancement},
  author={Cai, Yuanhao and others},
  booktitle={ICCV},
  year={2023}
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
