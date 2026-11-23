# Final Dataset

This folder contains the metadata file and access links to the processed RDD2022 dataset used in the RoadGuard project. The image and annotation files are hosted on Google Drive because their size is too large to store in this GitHub repository.

The images were resized while preserving their aspect ratio so that the longest dimension does not exceed 512 pixels, then converted to grayscale. The corresponding annotations are provided in YOLO format.

## Contents

- `Metadata.csv`: image identifiers, dataset split, file paths, original and resized dimensions, and resizing scale factors.
- **Development set:** training and validation images and their annotation files, used for development and parameter selection.
- **Test set:** 900 images and their annotation files, reserved for final evaluation.

The Google Drive folders are shared as **Anyone with the link – Viewer**. Use the links below to access the datasets.
## Development set
(https://drive.google.com/drive/folders/1d_t3ntdEc4yshN6p2JFv6sqcIsWrpfSt?usp=sharing)

## Test set
(https://drive.google.com/drive/folders/1RydE7DvWHIluHlqGoTyDTlHPafLvEUp3?usp=sharing)
