# 🚗 Vehicle Detection Using Classical Computer Vision

A computer vision pipeline that identifies and tracks vehicles in dashcam footage using traditional machine learning techniques. This project blends feature engineering, sliding window detection, and heatmap-based filtering to build a functional car detector—no deep learning involved!

![vehicle-detection-banner](images/detection_banner.jpg) <!-- Optional: add a visual banner -->

---

## 📌 Project Summary

This project demonstrates a vehicle detection pipeline using handcrafted image features (HOG, color histograms, spatial binning) and a Linear Support Vector Machine (SVM) classifier. It's designed to process road video footage and annotate vehicles in real time.

This is a modern implementation of classic vision techniques, built to better understand the foundations of autonomous vehicle perception systems.

---

## 🔍 Key Features

- ✅ HOG (Histogram of Oriented Gradients) for capturing object structure
- ✅ Color-based features to enrich classification
- ✅ Linear SVM classifier trained on labeled datasets
- ✅ Sliding window search across multiple scales
- ✅ Heatmap + thresholding to consolidate detections
- ✅ Video processing for frame-by-frame tracking

---

## 🧠 Technologies Used

- Python 3.x
- NumPy, OpenCV, Matplotlib
- scikit-learn (for ML modeling)
- MoviePy (for video handling)
- Jupyter Notebook

---

## 🛠️ How to Run

### 1. Clone this repo

```bash
git clone https://github.com/YOUR_USERNAME/vehicle-detection-classical-cv.git
cd vehicle-detection-classical-cv
```

### 2. Install dependencies

Use pip or conda to install requirements:

```bash
pip install -r requirements.txt
```

### 3. Train the classifier & run detection

Open the notebook:

```bash
jupyter notebook project.ipynb
```

Or run as a script (if modularized):

```bash
python src/train_classifier.py
python src/process_video.py
```

---

## 📂 Repository Layout

```
.
├── data/                   # Training datasets
├── images/                 # Sample input images
├── results/                # Output images and processed videos
├── src/                    # Python scripts and helper functions
│   ├── features.py
│   ├── detector.py
│   └── utils.py
├── model/                  # Trained classifier and scaler
├── project.ipynb           # Main notebook
├── requirements.txt
└── README.md
```

---

## 🎥 Sample Output

![demo](results/vehicle_detection_sample.gif)

---

## ✨ Improvements & Next Steps

- Add hard negative mining to improve classifier robustness
- Integrate temporal smoothing across video frames
- Benchmark with YOLO or Haar Cascades for performance comparison
- Explore false positive suppression using image pyramids

---

## 📚 Learnings

- The effectiveness of classical CV methods even in today's DL-dominated world
- The role of feature scaling and data preparation in traditional ML pipelines
- Practical insights into debugging detection pipelines using visual outputs

---

## 🧭 Acknowledgments

This project is inspired by a concept from the Udacity Self-Driving Car Nanodegree, adapted and restructured with custom enhancements, new documentation, and modular code organization.

---

## 🔗 Connect With Me

If you're working on similar projects or exploring classical ML in computer vision, I'd love to connect!

[LinkedIn](https://www.linkedin.com/in/YOUR_LINKEDIN) | [GitHub](https://github.com/YOUR_USERNAME)
