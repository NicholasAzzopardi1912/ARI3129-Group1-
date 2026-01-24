# ARI3129 – Assignment Materials  
**Traffic Sign Detection for Sign Type, Sign Viewing Angle Attribute, and Analytics using RF-DETR and YOLOv11**

This repository contains the materials submitted for the ARI3129 Computer Vision group assignment.  
The project focuses on traffic sign detection and the generation of post-detection analytics to support traffic sign monitoring and maintenance.

---

## Directory Structure Overview

```text
ARI3129 - Assignment Materials/
│
├── data/
│   ├── RF_DETR/
│   │   └── Dataset used for RF-DETR sign viewing angle detection
│   └── YOLO_COCO/
│       └── Dataset used for YOLOv11 sign type detection
│
├── runs/
│   ├── RF_DETR/
│   │   ├── predict/
│   │   ├── train/
│   │   │   ├── eval/
│   │   │   │   ├── BoxF1_curve.png
│   │   │   │   ├── BoxP_curve.png
│   │   │   │   ├── BoxPR_curve.png
│   │   │   │   ├── BoxR_curve.png
│   │   │   │   ├── curve_metrics.csv
│   │   │   │   └── labels.jpg
│   │   │   ├── checkpoint_best_total.pth
│   │   │   ├── log.txt
│   │   │   ├── metrics_plot.png
│   │   │   └── results.json
│   │   ├── confusion_matrix_normalized.png
│   │   ├── confusion_matrix.csv
│   │   ├── confusion_matrix.png
│   │   └── test_prediction_coco.json
│   └── YOLO/detect
│       ├── predict/
│       ├── runs/
│       │   └── train/
│       │       ├── yolov11_experiment/
│       │       │   ├── weights/
│       │       │   │   ├── best.pt
│       │       │   │   └── last.pt
│       │       │   ├── args.yaml
│       │       │   ├── BoxF1_curve.png
│       │       │   ├── BoxP_curve.png
│       │       │   ├── BoxPR_curve.png
│       │       │   ├── BoxR_curve.png
│       │       │   ├── confusion_matrix_normalized.png
│       │       │   ├── confusion_matrix.png
│       │       │   ├── events.out.tfevents.*   (TensorBoard logs)
│       │       │   ├── labels.jpg
│       │       │   ├── results.csv
│       │       │   ├── results.png
│       │       │   ├── train_batch0.jpg
│       │       │   ├── train_batch1.jpg
│       │       │   ├── train_batch2.jpg
│       │       │   ├── val_batch0_labels.jpg
│       │       │   ├── val_batch0_pred.jpg
│       │       │   ├── val_batch1_labels.jpg
│       │       │   ├── val_batch1_pred.jpg
│       │       │   ├── val_batch2_labels.jpg
│       │       │   ├── val_batch2_pred.jpg
│       │       └── val/
│       │           ├── eval_best_test/
│       │           ├── BoxF1_curve.png
│       │           ├── BoxP_curve.png
│       │           │   ├── BoxPR_curve.png
│       │           │   ├── BoxR_curve.png
│       │           │   ├── confusion_matrix_normalized.png
│       │           │   ├── confusion_matrix.png
│       │           │   ├── val_batch0_labels.jpg
│       │           │   ├── val_batch0_pred.jpg
│       │           │   ├── val_batch1_labels.jpg
│       │           │   ├── val_batch1_pred.jpg
│       │           │   ├── val_batch2_labels.jpg
│       │           │   └── val_batch2_pred.jpg
│       │           └── eval_yolov11_test/
│       │               ├── BoxF1_curve.png
│       │               ├── BoxP_curve.png
│       │               ├── BoxPR_curve.png
│       │               ├── BoxR_curve.png
│       │               ├── confusion_matrix_normalized.png
│       │               ├── confusion_matrix.png
│       │               ├── val_batch0_labels.jpg
│       │               ├── val_batch0_pred.jpg
│       │               ├── val_batch1_labels.jpg
│       │               ├── val_batch1_pred.jpg
│       │               ├── val_batch2_labels.jpg
│       │               └── val_batch2_pred.jpg
│       └── val/
│           ├── BoxF1_curve.png
│           ├── BoxP_curve.png
│           ├── BoxPR_curve.png
│           ├── BoxR_curve.png
│           ├── confusion_matrix_normalized.png
│           ├── confusion_matrix.png
│           ├── val_batch0_labels.jpg
│           ├── val_batch0_pred.jpg
│           ├── val_batch1_labels.jpg
│           ├── val_batch1_pred.jpg
│           ├── val_batch2_labels.jpg
│           └── val_batch2_pred.jpg
│
├── .gitignore
├── 1_data_visualisation.ipynb
├── 2a_[YOLOv11]_[Jeremy_Galea].ipynb
├── 2b_[RF-DETR_viewing_angle]_[Jeremy_Galea].ipynb
├── Dependencies.yml
└── README.md
```



---

## Notebooks

- **2a_[YOLOv11]_[Jeremy_Galea].ipynb**  
  Implements training, evaluation, and analytics generation for traffic sign **type** detection using YOLOv11.

- **2b_[RF-DETR_viewing_angle]_[Jeremy_Galea].ipynb**  
  Implements training, evaluation, and analytics generation for traffic sign **viewing angle** detection using RF-DETR.

---
## Trained Models

- RF-DETR's trained model **checkpoint_best_total.pth** is uploaded in the google drive: https://drive.google.com/drive/u/1/folders/1IcZum3eHyHb4qXCNPpZBUQoJWi1L7GWo
  - This should be placed in **.\runs\RF_DETR\train** if evaluation is to be run again. 

- YOLOv11's trained model **best.pt** is uploaded in its respective directory in **.\runs\YOLO\detect\runs\train\yolov11_experiment\weights**.

## Environment

- **Dependencies.yml** specifies the Conda environment used during development and experimentation.

---

## Author

**Jeremy Galea**  
B.Sc. (Hons) Artificial Intelligence  
University of Malta