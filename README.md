# Improved YOLOv5 with CBAM + C3TR for Small Object Detection (Floating Water Bottles)

This project extends the YOLOv5 object detection framework with CBAM (Convolutional Block Attention Module) and C3TR transformer blocks to improve **small object detection**, specifically targeting floating water bottle detection.

The workflow is designed to run in Google Colab and demonstrates training and inference using a modified YOLOv5 architecture.

---

## 🚀 Overview

* Base model: YOLOv5 (Ultralytics)
* Enhancements:

  * CBAM attention modules
  * C3TR transformer blocks
* Application: Floating water bottle detection
* Environment: Google Colab

---

## ⚙ Setup & Running the Notebook

1. Open the notebook:

   ```
   Yolov5x_CBAM_Trans_Floating_Bottles_Colab.ipynb
   ```

2. Run cells sequentially.

3. The default YOLOv5 repository will be cloned automatically.

---

## 🔁 Required File Replacements

Before training, replace the default YOLOv5 files with the modified versions in this repository:

```
yolov5/models/yolov5x.yaml
yolov5/models/common.py
yolov5/utils/loss.py
```

These files implement the CBAM + C3TR architecture.

---

## 📂 Dataset Requirements

The notebook expects a YOLO-format dataset structured as:

```
dataset/
 ├── images/train
 ├── images/val
 ├── labels/train
 └── labels/val
```

A dataset YAML file should define dataset paths and class labels.

> The dataset used for this academic project is not included due to size and storage limitations.

---

## 🔍 Training & Inference

You may:

* Train using your own dataset
* Load custom pretrained weights for inference

Place weights in:

```
weights/
```

and update paths inside the notebook.

---

## 📌 Notes

* Google Colab GPU runtime is recommended.
* Dataset paths inside the notebook may require editing.
* This repository focuses on architectural experimentation rather than dataset distribution.

---

## 📜 Credits

Based on YOLOv5 by Ultralytics.
Architecture modifications implemented for academic research.

---

## ✨ Author

Academic exploration of attention-enhanced object detection for environmental monitoring applications.