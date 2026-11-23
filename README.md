RoadGuard: Road-Damage Detection with Classical Image Processing and YOLO11

A Comparative Study Using the RDD2022 Dataset

Course: [Course name]

Instructor: [Instructor name]

Group: [Group number]

Project members: [Names of group members]


Overview

The classical pipeline enhances grayscale images, applies adaptive Gaussian thresholding and morphological operations, then uses a road-focused region of interest, connected-component analysis, and bounding-box extraction to produce damage candidates. YOLO11 directly predicts road-damage bounding boxes and classes. Both approaches are described in their respective sections of this repository.

Methods

Classical image processing: adaptive Gaussian thresholding, morphological operations, ROI filtering, connected-component analysis, and bounding-box extraction.
YOLO11: fine-tuning a pretrained detector, selecting a checkpoint using validation data, and evaluating it on the held-out Test Set.

Team and Contributions

| Member | Contribution |
|---|---|
| Member 1 | [Contribution] |
| Member 2 | Canny baseline |
| Member 3 | Image enhancement |
| Member 4 | Classical pipeline |
| Member 5 | Final evaluation and comparison |

Dataset

| Split | Images | Purpose |
|---|---:|---|
| Development Set | 5,100 | Development, configuration selection, and validation |
| Test Set | 900 | Final evaluation after settings are fixed |

The project uses road images and bounding-box annotations from RDD2022. Dataset access and preparation instructions are available [here]([dataset link]).


How to Reproduce a Run

1-Open the relevant notebook in Google Colab.

2-Follow the dataset access instructions in data/README.md.

3-Confirm that the notebook paths point to the required dataset folders.

4-Run the notebook cells in order.

5-Use the Test Set only for final evaluation after the method settings are fixed.
