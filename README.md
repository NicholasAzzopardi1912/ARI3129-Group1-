# ARI3129 – Assignment Materials  
**Traffic Sign Detection for Sign Type, Sign Condition Attribute, and Analytics using RetinaNet and YOLOv12**

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
│       │   └── Dataset used for RetinaNet sign type detection
│       └── YOLO_COCO_condition/
│           └── Dataset used for YOLOv12 sign condition detection
│
├── 2b_results
│	 ├── test_condition_analytics.csv - used for getting more results
│	 └── test_condition_analytics.json - used for getting more results
│
│
├── runs/
│   └── detect/
│       ├── predict/
│       │     └── jpg images of all test predictions     
│       │   
│       │
│       ├── train/
│       │
│       ├── train2/
│       │   
│       ├── train3/  
│       │
│       ├── train4/
│       │    └── results.csv 
│       │    └── results.png
│       │    └── labels.jpg
│       │    └── confusion_matrix_normalized.png
│       │    └── confusion_matrix.png
│       │    └── Box[F1, P, PR, R]_curve.png  
│       │    └── val_batch[0-2]_labels.jpg
│       │    └── val_batch[0-2]_pred.jpg
│       │    └── training_loss_plot.png
│       │    └── train_batch[0-2, 2601-2602].jpg
│       │    └── weights/
│       │          └── best.pt
│       │          └── last.pt
│       │
│       ├── val/
│       │    └── confusion_matrix_normalized.png
│       │    └── confusion_matrix.png
│       │    └── Box[F1, P, PR, R]_curve.png  
│       │    └── val_batch[0-2]_labels.jpg
│       │    └── val_batch[0-2]_pred.jpg
│       │    └── training_loss_plot.png
│       │    └── train_batch[0-2, 2601-2602].jpg   
│       │
│       └── val2/
│            
├── retinanet_best.pth           
├── retinanet_custom.pth          
│
├── 2a_[RetinaNet]_[Jamie].ipynb
├── 2b_[Yolov12_Sign_Condition]_[Jamie].ipynb
│
├── Dependencies.yml
├── yolo12n.pt
└── README.md
```



---

## Notebooks

- **2a_[RetinaNet]_[Jamie].ipynb**  
  Implements training, evaluation, and analytics generation for traffic sign **type** detection using RetinaNet.

- **2b_[Yolov12_Sign_Condition]_[Jamie].ipynb**  
  Implements training, evaluation, and analytics generation for traffic sign **condition** detection using YOLOv12.

---

## Analytics and Results

- **2a_[RetinaNet]_[Jamie].ipynb** contains RetinaNet post-detection analytics, including metrics, detected sign types, and qualitative prediction images.
- **2b_results/** contains YOLOv12 post-detection analytics, including per-image sign counts, detected sign conditions, and qualitative prediction images.
- Model performance metrics and training artefacts are stored within the corresponding model run directories.

---

## Environment

- **Dependencies.yml** specifies the Conda environment used during development and experimentation.

---

## Author

**Jamie Bugeja**  
B.Sc. (Hons) Artificial Intelligence  
University of Malta