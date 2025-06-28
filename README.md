# Thermal Human Detection using YOLOv8

## Overview

This repository presents a deep learning pipeline for **human detection in long-wave infrared (LWIR) thermal images** using **YOLOv8**, optimized for **border surveillance and intrusion detection** applications.

The model is trained on a custom thermal dataset that includes people moving under **low-light**, **foggy**, and **rainy** conditions, simulating real-world scenarios for automatic monitoring systems.

---

## Features

* **YOLOv8-Based Detection**  
  - Utilizes Ultralytics’ YOLOv8 for robust object detection.  
  - Fine-tuned for thermal imagery with high precision on small and low-contrast targets.

* **Custom Thermal Dataset**  
  - Recorded in forest environments using thermal cameras.  
  - Includes humans in various postures (standing, crouched) and motion types (walking, running).  
  - Weather conditions include clear nights, fog, and rain.

* **High Accuracy Performance**  
  - Achieved **>99% precision** and **mAP@0.5 = 0.992**.  
  - Robust to environmental noise, motion blur, and small-object visibility.

* **Colab-Ready Notebook**  
  - Includes scripts for visualization and batch inference.  
  - Lightweight and efficient model deployment.

---

## Dataset

The dataset is structured in **YOLO format** with separate folders for images and labels:


### `thermal_dataset.yaml` format:
```yaml
train: data/yolo_ready_dataset/images/train
val: data/yolo_ready_dataset/images/val

nc: 2
names: ['Human', 'Dog']

You can edit names as per your classes.I had dataset with humans and dogs so labelled accordingly
```
---

## How to Use

### 1. Clone the Repository

bash
git clone https://github.com/Vanshika070705/yolo_based_human_detection_from_thermal_images.git

cd thermal-yolo


### 2. Set Up Environment

* Use **Google Colab** or a **local environment** with **Python ≥ 3.8**  
* Install required dependencies:

```bash
pip install ultralytics opencv-python matplotlib
```

### 3. Run Inference Script

## Author

**[Vanshika Malik](https://github.com/Vanshika070705)**

This project was developed as part of a deep learning exploration into **thermal imaging for smart surveillance**.

hope you found it helpful :) <3



