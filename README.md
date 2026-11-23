# RoadGuard: Road-Damage Detection with Classical Image Processing and YOLO11

## A Comparative Study Using the RDD2022 Dataset

### Course: ARTI 403

### Instructor: Manal Almaeen

### Group: G3

### Project members: | Zainab Zaki Almajdi | Faridah Hussain Abdulaziz |Zainab Ali Alfaraj |  Joud Muhannad Alsaba | Salma Abdulelah Almuhanna



## Overview

The classical pipeline enhances grayscale images, applies adaptive Gaussian thresholding and morphological operations, then uses a road-focused region of interest, connected-component analysis, and bounding-box extraction to produce damage candidates. YOLO11 directly predicts road-damage bounding boxes and classes. Both approaches are described in their respective sections of this repository.

## Methods

Classical image processing: adaptive Gaussian thresholding, morphological operations, ROI filtering, connected-component analysis, and bounding-box extraction.
YOLO11: fine-tuning a pretrained detector, selecting a checkpoint using validation data, and evaluating it on the held-out Test Set.

## Team and Contributions

| Member | Contribution |
|---|---|
| Zainab Zaki Almajdi | Project proposal, objectives |
| Faridah Hussain Abdulaziz | Canny baseline and related edge-based experiments  |
| Zainab Ali Alfaraj | Image enhancement- Grayscale conversion and image enhancement |
| Joud Muhannad Alsaba | Classical damage-detection pipeline |
| Salma Abdulelah Almuhanna | Final evaluation, metrics, and results comparison |

## Dataset

| Split | Images | Purpose |
|---|---:|---|
| Development Set | 5,100 | Development, configuration selection, and validation |
| Test Set | 900 | Final evaluation after settings are fixed |

The project uses road images and bounding-box annotations from RDD2022. Dataset access and preparation instructions are available (https://github.com/sekilab/RoadDamageDetector).


## Repository Structure

```text
RoadGuard-Project/
├── Dataset/
│   └── final/
│       ├── Metadata.csv
│       └── README.md
├── YOLOv11/
│   ├── README.md
│   ├── RoadGuard_YOLO.ipynb
│   ├── RoadGuard_YOLO11.zip
│   └── best.pt
├── notebooks/
│   ├── RoadGuard_FINAL_(1)_(5).ipynb
│   └── classical_pipeline/
├── results/
│   └── classical_pipeline/
│       ├── Member3_Figures_improved-20261123T175916Z-1-001.zip
│       ├── Member4_Improved_Results-20261123T175926Z-1-001.zip
│       ├── Member4_Improved_Results_improved-20261123T175933Z-1-001.zip
│       ├── Member4_Improved_v2_Results-20261123T175952Z-1-001.zip
│       ├── RoadGuard_Canny_Baseline_improved-20261123T175956Z-1-001.zip
│       ├── RoadGuard_Member4_Masks_iou50_v4-20261123T180358Z-1-001.zip
│       └── README.md
└── README.md
```


## How to Reproduce a Run

1-Open the relevant notebook in Google Colab.

2-Follow the dataset access instructions in data/README.md.

3-Confirm that the notebook paths point to the required dataset folders.

4-Run the notebook cells in order.

5-Use the Test Set only for final evaluation after the method settings are fixed.
