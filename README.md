# MSFusion: Fine Fusion of Different Resolution SAR-Optical Images via Morphological Feature Decomposition

This repository accompanies the paper:

**Fine Fusion of Different Resolution SAR-Optical Images via Morphological Feature Decomposition**

## Authors
Wenfei Zhang, Yongxiang Yao*, Peihao Wu, Ruipeng Zhao, Bohan Sun, Yi Wan, Yongjun Zhang*  

School of Remote Sensing and Information Engineering, Wuhan University, Wuhan 430079, China  

📧 Corresponding authors:  
- Yongjun Zhang: zhangyj@whu.edu.cn  
- Yongxiang Yao: yaoyongxiang@whu.edu.cn  

---

## 📌 Overview

Due to substantial differences in **imaging mechanisms**, **spatial resolution**, and **noise characteristics** between Synthetic Aperture Radar (SAR) and optical images, fusing multi-resolution SAR–optical data remains highly challenging. Common fusion methods often suffer from **structural distortion**, **detail loss**, and **noise amplification**, especially under heterogeneous resolution conditions.

To address these issues, we propose **MSFusion**, a fine fusion framework for **different-resolution SAR–optical images**, based on **morphological feature decomposition** and **sparse detail compensation**.

---

## ✨ Key Contributions

The proposed MSFusion method introduces two major innovations:

### 1️⃣ Multi-level Morphological Feature Decomposition and Complementary Fusion
- A **differentiated multi-level feature decomposition framework** is designed.
- Morphological feature information is explicitly introduced to guide fusion.
- An **adaptive SSIM–AG weighting mechanism** is proposed to balance:
  - Noise suppression
  - Structural consistency
  - Detail preservation

### 2️⃣ Edge-Preserving Enhancement and Sparse Detail Compensation
- An **edge-preserving factor** is constructed using a **Sub-window Standard deviation Filter (SSF)**.
- **Robust Principal Component Analysis (RPCA)** and **K-SVD dictionary learning** are employed for sparse detail compensation.
- This strategy effectively suppresses high-frequency noise while recovering fine texture and edge details.

---

## 🗂️ Dataset: MultiRes-OSFusion

To comprehensively evaluate fusion performance, we construct the **MultiRes-OSFusion dataset**, which includes:

- **Over 2000 SAR–optical image pairs**
- SAR resolutions: **10 m** and **1 m**
- Coverage of **6 typical scene categories**
- Designed specifically for **cross-resolution SAR–optical fusion evaluation**

---

## 📊 Experimental Results

Extensive experiments demonstrate that **MSFusion consistently outperforms mainstream fusion methods** across multiple quantitative metrics, including:

- **Entropy (EN)**: +1.56%
- **Standard Deviation (SD)**: +7.89%
- **Spatial Frequency (SF)**: +20.46%
- **Average Gradient (AG)**: +16.93%

Compared to the best existing methods, MSFusion achieves a superior balance between:
- Structural preservation
- Texture and detail recovery
- Noise suppression

These results confirm the robustness and applicability of the proposed method for multi-resolution SAR–optical image fusion.

---

## 🔧 Code Availability

🚧 **The source code will be released publicly after paper acceptance.**  
Please stay tuned for updates.

If you are interested in early access, collaboration, or dataset usage, feel free to contact the authors.

---

## 📜 Citation

If you find this work useful in your research, please consider citing our paper:

```bibtex
@article{ZhangMSFusion2025,
  title={Fine Fusion of Different Resolution SAR-Optical Images via Morphological Feature Decomposition},
  author={Zhang, Wenfei and Yao, Yongxiang and Wu, Peihao and Zhao, Ruipeng and Sun, Bohan and Wan, Yi and Zhang, Yongjun},
  journal={},
  year={2025}
}
