# Multi-Expert Anatomy-Guided Negotiation (MEAG) for Object Detection in Fetal Echocardiography


This repository provides the official project page for:

**Multi-Expert Anatomy-Guided Negotiation (MEAG) for Object Detection in Fetal Echocardiography**


## Overview

Fetal echocardiographic object detection is challenging due to variations in cardiac structure size, low contrast, ambiguous boundaries, and dense spatial overlap.

We propose Multi-Expert Anatomy-Guided Negotiation (MEAG), an object-detection framework that separates candidate generation from candidate selection.

MEAG combines complementary candidates with anatomy-guided arbitration to improve detection of fetal cardiac structures, particularly those with weak visual evidence.


## Method

MEAG consists of four main components:

- **Dual-expert Candidate Generation**

  Combines the original YOLO26m-OBB prediction path with an additional detail path to generate complementary oriented bounding-box candidates.

- **Anatomical Policy Distillation**

  Uses teacher decisions and training annotations to provide supervision for candidate ranking.

- **Learned Anatomical Arbitration**

  Learns to rank competing candidates using detector confidence, rotated geometry, and anatomical relations.

- **Evidence-aware Safeguard**

  Retains the detector-confidence candidate when replacement evidence is insufficient.


## Results

MEAG was evaluated on 300 four-chamber fetal echocardiograms with 15 annotated classes.

Compared with YOLO26m-OBB, MEAG achieved:

- mAP50 improvement from 0.704 to 0.750
- Weak-structure mAP50 improvement from 0.449 to 0.539


## Paper

**Multi-Expert Anatomy-Guided Negotiation (MEAG) for Object Detection in Fetal Echocardiography**

Authors:

Yuyuan Bao, Camilla Fazi, Federica Fontanella, Netzahualcoyotl Hernandez-Cruz


## Code Availability

The source code will be released after the publication process is completed.



