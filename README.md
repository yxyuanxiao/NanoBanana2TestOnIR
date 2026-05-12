<div align="center">

# Can Nano Banana 2 Replace Traditional Image Restoration Models?  
## An Evaluation of Its Performance on Image Restoration Tasks

</div>

<div align="center">
  <a href="https://arxiv.org/abs/2604.03061"><img src="https://img.shields.io/badge/arXiv-2604.03061-b31b1b.svg" alt="Paper">
  <a href="https://drive.google.com/drive/folders/1n-8sTo1OgN96dZuAWCdYVPaPaMVMSDl8?usp=drive_link"><img src="https://img.shields.io/badge/Google%20Drive-Dataset-4285F4.svg?logo=googledrive&logoColor=white" alt="Google Drive"></a>
  <a href="https://pan.quark.cn/s/b31275a7f7e2"><img src="https://img.shields.io/badge/Quark%20Netdisk-Dataset-00CCFF.svg?logo=icloud&logoColor=white" alt="Quark Netdisk">
  </a>
  
</div>

<div align="center">
  <p>
    Weixiong Sun<sup>1</sup>,
    Xiang Yin<sup>2</sup>,
    <a href="https://scholar.google.com.hk/citations?user=OSDCB0UAAAAJ">Chao Dong</a><sup>31</sup>
  </p>
</div>

<div align="center">
  <sup>1</sup>Shenzhen University of Advanced Technology &nbsp;&nbsp;
  <sup>2</sup>Fudan University <br>
  <sup>3</sup>Shenzhen Institutes of Advanced Technology, Chinese Academy of Sciences
</div>

<br>

## 📢 News

- **[2026/05/12]** 🎉 Dataset is now publicly available on Google Drive and Quark Netdisk.
- **[2026/04]** 🎉 Our paper is available on [**arXiv:2604.03061**](https://arxiv.org/abs/2604.03061).
- **[2026/04]** 🎉 Our paper has been accepted to **CVPR 2026 Workshop AAVM**.
- **[2026/04/03]** Repository initialized.

## 📝 Overview

This repository accompanies the paper:

> **Can Nano Banana 2 Replace Traditional Image Restoration Models?  
> An Evaluation of Its Performance on Image Restoration Tasks**

While general-purpose image editing models like **Nano Banana 2** show promise as unified restoration solvers, our systematic study reveals a complex trade-off between perceptual appeal and reconstruction fidelity.

### 🔍 Key Research Focus

We conduct a systematic evaluation of Nano Banana 2 across diverse scenes and degradations to assess its potential as a unified restorer.

#### **Image Degradation Types (7 Types)**
We evaluate the model against both common optical distortions and realistic quality loss:
* **Blur Artifacts**: Defocus Blur, Motion Blur
* **Low-Quality Imaging**: Digital Zoom, Surveillance
* **Historical & Analog**: Old Film, Old Photo (Black and White), Old Photo (Color)

#### **Comprehensive Scene Categories (13 Types)**
Our dataset covers a wide array of visual structures, ranging from natural textures to complex semantic patterns:
* **Human-Centric**: Large Face, Medium Face, Small Face, Crowd, Hands/Feet
* **Natural & Textural**: Animal Fur, Trees/Leaves, Fabric Texture
* **Man-Made & Artistic**: Architecture, Text, Cartoon/Comic, Hand-drawn
* **Aerial Perspective**: Aerial View


#### **Core Research Objectives**
* **Unified Capability**: Assessing if a single general-purpose generative model can subsume specialized low-level vision systems.
* **Prompt Engineering**: Investigating how prompt length and explicit fidelity constraints (using 12 unique prompt designs) influence restoration outcomes.
* **Stability & Reliability**: Measuring model consistency across repeated inferences using statistical tests and identifying specific failure modes like hallucination and over-generation.
* **Comparison with SOTA**: Evaluating Nano Banana 2 against state-of-the-art restoration models (e.g., HYPIR, TSD-SR) to determine its standing in terms of both reconstruction fidelity and perceptual quality.

### 💡 Main Findings

* **Prompt Strategy**: Long prompts generally outperform short ones. However, concise prompts with **explicit fidelity instructions** provide the most effective guidance for balancing reconstruction accuracy and visual quality.
* **The Perception-Fidelity Gap**: Nano Banana 2 is consistently preferred in user studies due to its ability to produce sharp, visually rich textures. However, it tends to over-enhance details, leading to **infidelity** (semantic drift) and **over-generation** (unrealistic patterns).
* **Scenario Performance**: The model demonstrates superior performance in challenging tasks like **text restoration** (improving legibility) and **surveillance enhancement**, though it may sacrifice pixel-level consistency.
* **Evaluation Misalignment**: Existing IQA metrics and user studies often fail to capture semantic inconsistencies or color deviations, highlighting the need for more fidelity-aware evaluation protocols.

## 📦 Dataset

The dataset can be downloaded from either of the following sources:

| Source | Link |
| :--- | :--- |
| Google Drive | [Download](https://drive.google.com/drive/folders/13rqCsIv7xYRCw7HJcr53WZAZ4Kpc1VFm?usp=sharing) |  |
| Quark Netdisk | [Download](https://pan.quark.cn/s/b31275a7f7e2) | 

### **What's inside?**
To ensure reproducibility and facilitate further research, our dataset provides comprehensive results and metadata covering:
* **Prompt Design Evaluation**: Complete restoration outputs generated using 12 different prompt formulations (Long/Short, with/without Fidelity Hints).
* **Output Stability Analysis**: Results from repeated inference trials used to measure model consistency and stochastic variations.
* **SOTA Comparisons**: Comparative restoration results against state-of-the-art models including HYPIR, TSD-SR, PiSA-SR, and DiffBIR across all 20 categories.

## 📚 Citation

If you find our work useful for your research, please consider citing:

```bibtex
@article{sun2026nano,
  title   = {Can Nano Banana 2 Replace Traditional Image Restoration Models? An Evaluation of Its Performance on Image Restoration Tasks},
  author  = {Sun, Weixiong and Yin, Xiang and Dong, Chao},
  journal = {arXiv preprint arXiv:2604.03061},
  year    = {2026}
}
```

## 📬 Contact

For questions or discussions, please open an issue in this repository.
