# Detection and Classification of Liver Cirrhosis 🩺🧠

An AI-powered medical imaging system for **automated detection, classification, and segmentation of liver cirrhosis and tumors** using **Ultrasound and CT scans**.  
This project provides a **non-invasive**, **accurate**, and **scalable** diagnostic tool to support clinicians and patients.

---

## 📌 Project Overview

Liver cirrhosis is a life-threatening condition that often goes undetected until advanced stages.  
Traditional diagnosis relies on **invasive liver biopsy** and **manual interpretation** of medical images.

This project proposes a **deep learning-based system** that:
- Classifies liver fibrosis stages (**F0 – F4**) from **ultrasound images**
- Segments liver and tumor regions from **CT scans**
- Generates clear visual and clinical reports through a user-friendly interface

---

## 🎯 Objectives

- Develop an automated system for **early detection** of liver cirrhosis
- Reduce dependency on invasive diagnostic procedures
- Assist doctors with **AI-based decision support**
- Provide a scalable solution suitable for **low-resource healthcare environments**

---

## 🧠 System Architecture

The system consists of the following main components:

1. **Data Acquisition**
   - Ultrasound images (fibrosis classification)
   - CT scans (liver & tumor segmentation)

2. **Image Preprocessing**
   - RGB conversion
   - Resizing to 224×224
   - Pixel normalization
   - Data augmentation
   - Class balancing

3. **Deep Learning Models**
   - Classification models (CNN-based)
   - Segmentation models (U-Net++)

4. **Backend APIs**
   - Flask / FastAPI services for inference

5. **User Interface**
   - Web & mobile interfaces for doctors and patients

---

## 🗂️ Datasets

### Ultrasound Dataset
- Classified according to **METAVIR scoring system**
- Fibrosis stages:
  - F0 (No fibrosis)
  - F1
  - F2
  - F3
  - F4 (Cirrhosis)

### CT Scan Dataset
- **LiTS (Liver Tumor Segmentation) Dataset**
- Includes ground truth masks for:
  - Liver
  - Tumors
  - Bones
  - Arteries
  - Kidneys

---

## 🤖 Models Used

### Classification Models
- ResNet-50
- VGG-19
- DenseNet-121 ✅ *(Best performing)*
- NASNetMobile
- InceptionResNetV2

### Segmentation Model
- **U-Net++ with EfficientNet-B5 encoder**

---

## 📊 Performance Highlights

| Task | Model | Accuracy |
|-----|------|---------|
| Fibrosis Classification | DenseNet-121 | **97.7%** |
| Liver & Tumor Segmentation | U-Net++ + EfficientNet-B5 | **97.9%** |

- High Precision, Recall, F1-score
- Strong AUC performance
- Robust generalization after augmentation and balancing

---
## 🎥 Demo Video

Watch a full demonstration of the system, including:
- Liver fibrosis classification (F0–F4)
- Liver & tumor segmentation
- Web & mobile application workflow




https://github.com/user-attachments/assets/561081f2-503a-4fe3-9235-bab14756c971


https://github.com/user-attachments/assets/9fd57911-f798-4a86-b84f-ae5672e7baab


## 🛠️ Technologies Used

### Programming & AI
- Python
- TensorFlow / Keras
- NumPy, OpenCV
- Matplotlib, Seaborn

### Backend
- Flask
- FastAPI
- Hugging Face integration

### Frontend
- Flutter (Mobile App)
- HTML & CSS (Web)

### Deployment
- Oracle APEX
- REST APIs

---

## 🧪 Features

- Upload ultrasound or CT images
- Automatic liver segmentation
- Fibrosis stage classification (F0–F4)
- Tumor detection
- Confidence scores
- Visual overlays for interpretability
- Medical report generation
- Liver health advice section

---


# Install dependencies
pip install -r requirements.txt

# Run backend
python app.py
