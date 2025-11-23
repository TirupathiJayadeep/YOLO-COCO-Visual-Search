# Computer Vision Powered Search Application using YOLOv11

##  Project Title
**Object Detection Based Image Search Engine Using YOLOv11 and Streamlit**

##  Abstract / Introduction
This project implements a **Computer Vision Search Engine** that allows users to search for images containing specific objects using **YOLOv11**, one of the most advanced object detection models.  
The system processes a directory of images, detects objects, and indexes metadata, enabling fast content-based image retrieval.

A simple and interactive front-end interface is created using **Streamlit**, and the system runs locally through **VS Code** inside a **Conda environment**.

##  Dataset & YOLO Model Details
- **Dataset used:** COCO Validation Dataset (coco-val-2017-500 subset)
- **Number of object classes:** 80 COCO categories
- **Model used:** YOLOv11m (`yolov11m.pt`)
- **Framework:** Ultralytics YOLO

##  Environment Setup (Required)
### **Conda environment creation**
```bash
conda create -n yolo_image_search_gpu python=3.11
conda activate yolo_image_search_gpu
```

### Install Dependencies (GPU Version)
'''
pip install "numpy<2" --force-reinstall --no-cache-dir
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu121
pip install opencv-python
pip install ultralytics
pip install streamlit
pip install pillow scipy psutil
'''

## Running the Application
### Step 1 — Activate Environment
```
conda activate yolo_image_search_gpu
```
### Step 2 — Run Streamlit
```
streamlit run app.py
```
### Step 3 — Open Browser
http://localhost:8501

## Application Usage
### 1.In the Streamlit UI:
### 2.Select Process new images
### 3.Enter the path to images, e.g.
C:\Users\admin\OneDrive\Desktop\Yolo11\coco-val-2017-500
### 4.Enter YOLO model weights path:
yolov11m.pt
### 5.Click Start Inference
### 6.Search for objects like.

## Results & Conclusion
This system successfully detects objects and retrieves relevant images based on object occurrences.

