# [ICML 2026] Crowd4D: Scene-Aware Monocular 4D Crowd Reconstruction

**[Hongbo Kang](https://khb1698.github.io/)**, **[Tianyi Zhou](#)**, **[Qingyang Yang](#)**, **[Hongwei Wen](#)**, **[Jing Huang](#)**, **[Yu-Kun Lai](https://yukunlai.github.io/)**, **[Kun Li](http://cic.tju.edu.cn/faculty/likun/)**<sup>🌟</sup>

🌟Corresponding Author

📄 **[Paper](https://icml.cc/virtual/2026/poster/65335)** | 🌍 **[Project Page](#)** | 💻 **[Code](https://github.com/KHB1698/Crowd4D)**

![Crowd4D Teaser](assets/Crowd4D.png)

---

## 📰 News

- **2026-05:** Paper accepted to ICML 2026! Code will be released soon.

---

## 📌 Features

- **Scene-Aware Reconstruction** – Joint optimization of crowd and scene from monocular video, handling complex, non-planar terrain.
- **Human-Scene Interaction Proxy (HSIP)** – A compact intermediate representation built on Scene Interaction Point Cloud (SIPC) and Scene Interaction Surface (SIS) that provides temporally stable geometric anchors.
- **Crowd Structural Coherence Regularization (CSCR)** – Enforces soft temporal consistency on pairwise relative displacements within local crowd neighborhoods, improving robustness under occlusions.
- **Multi-Stage Optimization** – Progressively refines global scale, root positions, articulated poses, and motion dynamics for stable and accurate results.

---

## 📖 Citation

If you find Crowd4D useful for your research, please cite:

```bibtex
@inproceedings{kang2026crowd4d,
  author = {Hongbo Kang, Tianyi Zhou, Qingyang Yang, Hongwei Wen, Jing Huang, Yu-Kun Lai and Kun Li},
  title = {Crowd4D: Scene-Aware Monocular 4D Crowd Reconstruction},
  booktitle = {International Conference on Machine Learning (ICML)},
  year={2026}
}
```

If you use DyCrowd, please cite:

```bibtex
@article{wen2025dycrowd,
  author = {Hao Wen, Hongbo Kang, Jian Ma, Jing Huang, Yuanwang Yang, Haozhe Lin, Yu-Kun Lai and Kun Li},
  title = {DyCrowd: Towards Dynamic Crowd Reconstruction from a Large-scene Video},
  journal = {IEEE Transactions on Pattern Analysis and Machine Intelligence},
  year={2025}
}
```

---

## � Acknowledgements

We thank the authors of [DyCrowd](https://github.com/KHB1698/DyCrowd) for their foundational work on dynamic crowd reconstruction.

## �📄 License

This project is released under the MIT License.
