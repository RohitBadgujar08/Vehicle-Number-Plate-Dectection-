
# 🚘 Automatic Number Plate Recognition (ANPR) for Indian Vehicles

This project implements an Automatic Number Plate Recognition (ANPR) system tailored for Indian vehicle license plates using classical image processing techniques and Optical Character Recognition (OCR). It is lightweight, efficient, and suitable for low-resource environments such as housing societies, parking lots, and institutional access control.

## 📸 Overview

The system processes video input to detect and recognize vehicle number plates using OpenCV and Tesseract OCR. It handles common challenges such as noise, skewed plates, and lighting variations without using deep learning models.

## 🔍 Features

- Real-time license plate detection from video
- Preprocessing using Gaussian smoothing and edge detection
- Contour-based license plate localization
- OCR-based alphanumeric text recognition using Tesseract
- Saves detected plates and annotated frames
- Lightweight, interpretable solution without machine learning

## 🧰 Technologies Used

- Python 3
- OpenCV
- Pytesseract (Tesseract OCR)
- NumPy
- PIL (Python Imaging Library)

## 🗂️ Project Structure

```
├── SIP_FINAL_PROJECT.ipynb        # Jupyter notebook with full implementation
├── /output                        # Folder to save detected plates and frames
├── /input_video                   # Folder to store test videos
├── README.md                      # This file
```

## 🧪 How It Works

1. **Video Input:** Captures video using OpenCV.
2. **Frame Preprocessing:** Grayscale conversion, noise removal (bilateral filtering), and edge detection.
3. **Contour Detection:** Extracts top contours and filters quadrilaterals (assumed license plates).
4. **Plate Extraction:** Isolates plate region using bounding boxes.
5. **Text Recognition:** Applies Tesseract OCR to extract alphanumeric text.
6. **Storage:** Saves both recognized plates and original annotated frames.

## ✅ Results

- Works on real-world video inputs under various lighting and noise conditions.
- Achieves around 70–80% accuracy on clear, standard plates.
- Handles noise, skew, and brightness through preprocessing.
- Lightweight and suitable for embedded or low-power applications.

## 📦 Applications

- Gated community vehicle access
- Parking management
- Toll booths
- Border control
- Traffic monitoring and enforcement

## ⚠️ Limitations

- Not suitable for heavily occluded or non-standard plates.
- Performance may drop with motion blur or extreme angles.
- No deep learning used—may not generalize to highly varied datasets.

## 🚀 Future Work

- Integrate deep learning-based detection (YOLO, CRNN) for robustness.
- Add a GUI dashboard for live feed monitoring.
- Extend to multilingual plates and state-wise plate pattern detection.

## 👥 Authors

- Aditya Shaju
- Rohit Badgujar
- Bhavesh Supe
- Aniket Sonkamble
- Vaibhav Gujarathi  
(*NMIMS University, Department of Information Technology*)

## 📄 License

This project is for academic and educational use. Please credit the authors when reusing or modifying the work.
