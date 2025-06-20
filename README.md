# YOLOv8 v3 – Custom Object Detection

This project demonstrates a custom object detection pipeline using **YOLOv8**, trained on a personalized dataset from **Kaggle**. The third version of the model includes improved performance, dataset enhancements, and refined training parameters.

---

## 🔍 Project Overview

- **Model**: YOLOv8 (Ultralytics)
- **Version**: v3 (best performing model so far)
- **Dataset**: Custom dataset (day and night images) uploaded and trained on **Kaggle**
- **Task**: Detect and classify objects (e.g., animals, vehicles, etc.)
- **Framework**: Python, PyTorch

---

## 🧠 Key Features

- Trained with **custom annotated dataset**
- Supports **real-time object detection**
- Version-controlled development (`v1`, `v2`, and current `v3`)
- Uses **Ultralytics YOLOv8** repo for architecture

---

## 🗃️ Folder Structure

YoloV8/
├── runs/
│ └── detect/
│ └── train3/ ← Output of v3 training
├── data/ ← YAML and dataset structure
├── weights/ ← best.pt model (not pushed if >100MB)
├── train.py ← Training script
├── predict.py ← Inference script
├── README.md ← This file


---

## 🚀 How to Use

1. **Clone this repo**:

```bash
git clone https://github.com/pranavmukundanA/Yolov8-v3.git
cd Yolov8-v3

2.Install YOLOv8:
pip install ultralytics

3.Train your model:
yolo detect train data=data.yaml model=yolov8n.pt epochs=50 imgsz=640

4.Run Inference:
yolo detect predict model=weights/best.pt source=your_video.mp4

5.Results:

| Metric    | Value  |
| --------- | -----  |
| Precision | 61.54% |
| Recall    | 93.85% |
| mAP\@0.5  | 64.13% |
| Avg IoU   | 55.16% |

6.Tech Stack
Python
YOLOv8 (Ultralytics)
PyTorch
Kaggle for training
Git & GitHub for version control


Let me know if you want:
- This saved and pushed for you
- A `.gitignore` to add next
- Help uploading `best.pt` using GitHub Releases
