# ARI3129 – Assignment Materials  
**Traffic Sign Detection for Sign Type, Sign Shape Attribute, and Analytics using Faster R-CNN and YOLOv8**

This repository contains the materials submitted for the ARI3129 Computer Vision group assignment.  
The project focuses on traffic sign detection and the generation of post-detection analytics to support traffic sign monitoring and maintenance.

---

## Directory Structure Overview

```text
ARI3129 - Assignment Materials/
│
├── Data/
│   └── Datasets/
│       ├── COCO-based_COCO/
│       │   └── Dataset used for Faster R-CNN sign type detection
│       └── YOLO_COCO_sign_shape/
│           └── Dataset used for YOLOv8 sign shape detection
│
├── runs/
│   └── ari3129/
│       ├── analytics_sign_shape/
│       │   ├── predictions/
│       │   ├── sign_shape_analytics.json
│       │   └── sign_shape_analytics.csv
│       │
│       ├── analytics_sign_type/
│       │   ├── predictions/
│       │   ├── sign_type_analytics.json
│       │   └── sign_type_analytics.csv
│       │
│       ├── fasterrcnn_sign_type_v1/
│       │   ├── best.pt (not included – exceeds GitHub 100 MB limit)
│       │   ├── history.json
│       │   └── test_metrics.json
│       │
│       └── yolov8_sign_shape_v1/
│           ├── weights/
│           ├── args.yaml
│           └── results.csv
│
├── 2a_[Faster R-CNN]_[Nicholas].ipynb
├── 2b_[Yolov8_Sign_Shape]_[Nicholas].ipynb
│
├── Dependencies.yml
└── README.md


---

## Notebooks

- **2a_[Faster R-CNN]_[Nicholas].ipynb**  
  Implements training, evaluation, and analytics generation for traffic sign **type** detection using Faster R-CNN.

- **2b_[Yolov8_Sign_Shape]_[Nicholas].ipynb**  
  Implements training, evaluation, and analytics generation for traffic sign **shape** detection using YOLOv8.

---

## Analytics and Results

- **analytics_sign_type/** contains Faster R-CNN post-detection analytics, including per-image sign counts, detected sign types, and qualitative prediction images.
- **analytics_sign_shape/** contains YOLOv8 post-detection analytics, including per-image sign counts, detected sign shapes, and qualitative prediction images.
- Model performance metrics and training artefacts are stored within the corresponding model run directories.

---

## Environment

- **Dependencies.yml** specifies the Conda environment used during development and experimentation.

---

## Author

**Nicholas Azzopardi**  
B.Sc. (Hons) Artificial Intelligence  
University of Malta