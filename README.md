# Waterfowl-Detection-Categorization-and-Count-Using-YOLO-and-Drone-Imagery-for-Wildlife-Conservation

# Waterfowl Detection and Count Using YOLOv8 and Drone Imagery for Wildlife Conservation

## Overview

This project focuses on automated detection and counting of flamingos from aerial drone imagery using YOLOv8. The objective is to support wildlife monitoring and conservation efforts by reducing the need for manual bird counting.

## Motivation

Traditional wildlife surveys are time-consuming and prone to human error. By leveraging drone imagery and deep learning, bird populations can be monitored efficiently over large wetland areas.

## Dataset

A custom dataset was created using drone imagery captured over flamingo habitats.

### Annotation

* Annotation Tool: CVAT
* Format: YOLO Bounding Boxes
* Species: Flamingo
* Viewpoint: Top-down Drone Imagery

Dataset samples are available in the `images/` directory.

Full dataset:

https://drive.google.com/drive/folders/1hhdCh31Ox5t7ozdtjwpH5gHvWD2DZgzS

## Methodology

### Data Preparation

* Manual annotation using CVAT
* Train / Validation split
* Quality verification of labels

### Model

* YOLOv8
* Transfer Learning
* Fine-tuned on custom flamingo dataset

## Results

| Metric    | Score  |
| --------- | ------ |
| Precision | 84.99% |
| Recall    | 84.08% |
| mAP@50    | 91.45% |
| mAP@50-95 | 75.54% |

The model achieved strong detection performance on unseen validation imagery.

## Training Curves

![Training Results](results/results.png)

## Precision Recall Curve

![PR Curve](results/BoxPR_curve.png)

## Confusion Matrix

![Confusion Matrix](results/confusion_matrix_normalized.png)

## Detection Examples

### Validation Predictions

![Prediction 1](predictions/val_batch0_pred.jpg)

![Prediction 2](predictions/val_batch1_pred.jpg)

![Prediction 3](predictions/val_batch2_pred.jpg)

## Technologies Used

* Python
* YOLOv8
* PyTorch
* OpenCV
* CVAT

## Applications

* Wildlife Conservation
* Bird Population Monitoring
* Ecological Surveys
* Wetland Management

## Future Work

* Multi-species bird detection
* Real-time drone deployment
* Bird tracking in video streams
* Migration pattern monitoring

## Author

Konark Karia
M.Tech – Data Science & AI
Research Intern, ISRO SAC
