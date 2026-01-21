# ARI3129 – Assignment Materials  
**Traffic Sign Detection for Sign Type, Sign Condition Attribute, and Analytics using YOLOv10 and EfficientDet**

This repository contains the materials submitted for the ARI3129 Computer Vision group assignment.  
The project focuses on traffic sign detection and the generation of post-detection analytics to support traffic sign monitoring and maintenance.

---

## Directory Structure Overview

```text
ARI3129 - Assignment Materials/
│
├── Best Models/
│   ├── best_mounting_model.pth
│   └── yolov10n.pt
│
├── runs/
│   ├── EfficientDet_Mounting_Eval/
│   │   └── events.out.tfevents...
│   └── YOLOv10_analytics/
│       ├── YOLO_SignType_v10/
│       ├── YOLO_SignType_v102/
│       ├── YOLO_SignType_v103/
│       ├── val/
│       ├── val2/
│       ├── val3/
│       └── val4/
│
├── 2a_[YOLOv10]_[Roman_Vasilets].ipynb
├── 2b_[EfficientDet_Sign_Mounting]_[Roman_Vasilets].ipynb
│
├── Dependencies.yml
│
├──Datasets/  ->  Found below in a google drive link
│   ├── COCO-based_COCO_mounting/
│   │      ├── annotations/
│   │      └── images/
│   │
│   └── YOLO_COCO/
│        ├── images/
│        ├── labels/
│        ├── data.yaml
│        └── data.yaml.json
│
└── README.md
```



---

## Notebooks

- **2a_[YOLOv10]_[Roman_Vasilets].ipynb**  
  Implements training, evaluation, and analytics generation for traffic sign **type** detection using YOLOv10.

- **2b_[EfficientDet_Sign_Mounting]_[Roman_Vasilets].ipynb**  
  Implements training, evaluation, and analytics generation for traffic sign **mounting** detection using EfficientDet.

---

## External Link to produced COCO and YOLO Datasets
- **https://drive.google.com/drive/folders/157w4JxNuwICgSLwZcuAcGR1DPMaDCuer?usp=drive_link**

---

## Analytics and Results

- **runs/** contains YOLOv10 post-detection analytics, the predicted test dataset images including per-image sign counts, detected sign conditions, and qualitative prediction images as well as for EfficientDet.
- Model performance metrics and training artefacts are stored within the corresponding model run directories.

---

## Environment

- **Dependencies.yml** specifies the Conda environment used during development and experimentation.

---

## Author

**Roman Vasilets**  
B.Sc. (Hons) Artificial Intelligence  
University of Malta
