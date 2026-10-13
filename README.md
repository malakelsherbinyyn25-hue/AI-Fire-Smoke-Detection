# 🔥 AI-Based Fire & Smoke Detection Using Deep Learning

## 📌 Project Overview

This project uses Deep Learning and the YOLOv8 object detection model to detect fire and smoke in images. The goal is to support early fire detection and improve safety through automated visual monitoring.

## 🎯 Project Objectives

* Detect fire and smoke using computer vision.
* Identify detected objects with bounding boxes.
* Train and evaluate a YOLOv8 model.
* Analyze model performance using evaluation metrics and visualization plots.

## 🛠️ Technologies Used

* Python
* YOLOv8
* Ultralytics
* Deep Learning
* Computer Vision
* Google Colab

## 🧠 Model Training Configuration

The model was trained using the following configuration:

| Parameter            | Value                 |
| -------------------- | --------------------- |
| Model                | YOLOv8n               |
| Classes              | Fire, Smoke           |
| Epochs               | 50                    |
| Image Size           | 640 × 640             |
| Batch Size           | 16                    |
| Training Environment | Google Colab with GPU |

## 📊 Model Evaluation

The YOLOv8 model was evaluated on the validation dataset containing 872 images and two classes: **Fire** and **Smoke**.

### Overall Evaluation Metrics

| Metric    |  Score |
| --------- | -----: |
| Precision | 76.95% |
| Recall    | 68.72% |
| mAP@50    | 73.82% |
| mAP@50-95 | 44.49% |

### Class-wise Evaluation

| Class | Precision | Recall | mAP@50 | mAP@50-95 |
| ----- | --------: | -----: | -----: | --------: |
| Fire  |     78.2% |  76.8% |  80.3% |     46.1% |
| Smoke |     75.7% |  60.6% |  67.3% |     42.8% |

### Training and Evaluation Visualizations

The repository includes:

* Precision-Recall curve
* Precision curve
* Recall curve
* F1-score curve
* Confusion matrix
* Normalized confusion matrix
* Training results across epochs

### Observations

The model achieved better detection performance for Fire than for Smoke. Smoke detection remains an area for improvement, particularly in Recall.

*Note: These results were obtained by evaluating the saved `best.pt` checkpoint on the validation dataset. Performance on unseen test data may differ.*


### Training and Evaluation Visualizations

The repository includes:

* Precision-Recall curve
* Precision curve
* Recall curve
* F1-score curve
* Confusion matrix
* Normalized confusion matrix
* Training results across epochs


## 📁 Repository Contents

* `best.pt` — Trained model weights.
* `results.csv` — Training metrics recorded across epochs.
* `results.png` — Training results visualization.
* `BoxPR_curve.png` — Precision-Recall curve.
* `BoxP_curve.png` — Precision curve.
* `BoxR_curve.png` — Recall curve.
* `BoxF1_curve.png` — F1-score curve.
* `confusion_matrix.png` — Confusion matrix.
* `confusion_matrix_normalized.png` — Normalized confusion matrix.
* Training notebook (`.ipynb`) — Notebook containing the training workflow.

## 🚀 Future Improvements

* Real-time fire and smoke detection using a webcam.
* Audio or message alerts when fire or smoke is detected.
* Integration with a user-friendly monitoring dashboard.
* Further testing under different lighting and environmental conditions.

## 👩‍💻 Project Focus

Model Training and Evaluation using YOLOv8 and Deep Learning.

---

**Note:** This project is developed for educational purposes. Its predictions should not be treated as a replacement for certified fire detection and safety systems.
