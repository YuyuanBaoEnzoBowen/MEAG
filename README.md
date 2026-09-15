# Multi-Expert Anatomy-Guided Negotiation (MEAG) for Object Detection in Fetal Echocardiography


## Overview

This repository is the official project page for:

**"Multi-Expert Anatomy-Guided Negotiation (MEAG) for Object Detection in Fetal Echocardiography"**

MEAG is an anatomy-guided object detection framework designed for fetal echocardiographic structure detection. It addresses challenges caused by small structures, weak visual evidence, ambiguous boundaries, and dense spatial overlap in fetal cardiac ultrasound images.


## Method

MEAG separates candidate generation from candidate selection through a multi-expert negotiation framework.

The framework consists of four components:

- **Dual-Expert Candidate Generation (DE-CGM)**  
  Generates complementary oriented bounding-box candidates using stable and detail proposal experts.

- **Anatomical Policy Distillation (APD)**  
  Converts anatomical reasoning into supervision signals for candidate ranking.

- **Learned Anatomical Arbitration (LAA)**  
  Learns to select better candidates using detector confidence, rotated geometry, and anatomical relations.

- **Evidence-aware Safeguard**  
  Maintains conservative decisions when anatomical evidence is insufficient.


## Paper

**Multi-Expert Anatomy-Guided Negotiation (MEAG) for Object Detection in Fetal Echocardiography**

Authors:

Yuyuan Bao, Camilla Fazi, Federica Fontanella, Netzahualcoyotl Hernandez-Cruz


Conference:

IEEE International Conference on Biomedical Engineering and Systems (IBIOMED) 2026


## Results

MEAG was evaluated on fetal echocardiography object detection.

Compared with YOLO26m-OBB:

- mAP50 improved from 0.704 to 0.750
- Weak-structure mAP50 improved from 0.449 to 0.539

The results demonstrate improved detection performance, particularly for challenging anatomical structures.


## Code Availability

The source code and pretrained models will be released after the publication process is completed.


## Citation

If you find this work useful, please cite:

```bibtex
@inproceedings{bao2026meag,
  title={Multi-Expert Anatomy-Guided Negotiation (MEAG) for Object Detection in Fetal Echocardiography},
  author={Bao, Yuyuan and Fazi, Camilla and Fontanella, Federica and Hernandez-Cruz, Netzahualcoyotl},
  booktitle={IEEE International Conference on Biomedical Engineering and Systems},
  year={2026}
}
