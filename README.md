# [ICML 2026] Crowd4D: Scene-Aware Monocular 4D Crowd Reconstruction

**[Hongbo Kang](https://khb1698.github.io/)**<sup>🌟</sup>, **[Tianyi Zhou](#)**, **[Qingyang Yang](#)**, **[Hongwei Wen](#)**, **[Jing Huang](#)**, **[Yu-Kun Lai](https://yukunlai.github.io/)**, **[Kun Li](http://cic.tju.edu.cn/faculty/likun/)**<sup>🌟</sup>

🌟Corresponding Authors

📄 **[Paper](#)** | 🌍 **[Project Page](#)** | 💻 **[Code](https://github.com/KHB1698/Crowd4D)** | 📂 **[Datasets](#)**

![Crowd4D Teaser](assets/Crowd4D.png)

---

## 🎯 Key Features

- **First scene-aware monocular 4D crowd reconstruction** framework that jointly reconstructs 3D poses, positions, and shapes of multiple people from a single video while reasoning about scene context
- **Scene-grounded human modeling** that leverages monocular depth estimation and semantic scene parsing to anchor people in 3D space with physical plausibility
- **Temporally coherent 4D optimization** with scene-aware constraints (ground contact, collision avoidance, scene occupancy) for consistent crowd motion over time
- **Novel view synthesis** capability by lifting monocular crowd videos to a full 4D representation, enabling rendering from arbitrary viewpoints
- **State-of-the-art performance** on multiple crowd reconstruction benchmarks, significantly outperforming prior methods in both 3D accuracy and temporal consistency

---

## 📊 Datasets

We evaluate Crowd4D on the following datasets:

| Dataset | Description | Availability |
|---------|-------------|-------------|
| **VirtualCrowd-4D** | Extended VirtualCrowd benchmark with scene annotations and multi-view ground truth | Request upon publication |
| **Crowd4D-Synthetic** | Synthetic crowd scenes with varying density, camera motion, and scene complexity | Coming Soon |
| **Crowd4D-Real** | Real-world monocular crowd videos with scene scans | Coming Soon |

**Requesting the Dataset:** Please contact [hbkang@tju.edu.cn](mailto:hbkang@tju.edu.cn) to request access.

---

## 🏗️ Framework Overview

Crowd4D introduces a scene-aware monocular 4D crowd reconstruction pipeline consisting of three main modules:

1. **Scene Encoder** — Monocular depth estimation + semantic scene parsing → 3D scene representation
2. **Human Perception Network** — Multi-person 2D pose detection → Instance-aware feature extraction → 3D lifting with scene grounding
3. **4D Temporal Optimizer** — Scene-constrained motion prior → Temporally consistent 4D trajectory optimization

---

## 🚀 Getting Started

### Requirements

- Python 3.10+
- PyTorch 2.0+
- CUDA 11.8+

### Installation

```bash
git clone https://github.com/KHB1698/Crowd4D.git
cd Crowd4D
conda create -n crowd4d python=3.10
conda activate crowd4d
pip install -r requirements.txt
```

### Data Preparation

```bash
# Download dataset
# Place data in ./data/ with the following structure:
# data/
#   virtualcrowd-4d/
#   crowd4d-synthetic/
#   crowd4d-real/
```

### Training

```bash
python scripts/train.py --config configs/crowd4d.yaml
```

### Evaluation

```bash
python scripts/test.py --checkpoint path/to/checkpoint
```

### Demo

```bash
python scripts/demo.py --video path/to/video.mp4
```

---

## 📈 Results

<p align="center">
  <img src="assets/teaser.png" width="80%"/>
</p>

---

## 📖 Citation

If you find our work useful, please consider citing:

```bibtex
@inproceedings{kang2026crowd4d,
  author = {Hongbo Kang, Tianyi Zhou, Qingyang Yang, Hongwei Wen, Jing Huang, Yu-Kun Lai and Kun Li},
  title = {Crowd4D: Scene-Aware Monocular 4D Crowd Reconstruction},
  booktitle = {International Conference on Machine Learning (ICML)},
  year={2026}
}
```

---

## 📧 Contact

For questions or collaborations, please contact [hbkang@tju.edu.cn](mailto:hbkang@tju.edu.cn).

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
