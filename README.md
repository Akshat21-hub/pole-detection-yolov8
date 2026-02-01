# Pole Detection using YOLOv8

This project contains a computer vision model trained to **detect poles in images and classify them by color**:
- Blue pole
- Red pole
- Yellow pole

The model is trained using **YOLOv8 (Ultralytics)** on a Roboflow poles dataset and can be tested on any new images.

---

## 📌 Classes Detected
- `bluep`  – Blue pole  
- `redp`   – Red pole  
- `yellowp`– Yellow pole  

---

## 📦 Files in this Repository
- `best.pt` – Trained YOLOv8 model weights  
- `data.yaml` – Dataset configuration  
- `Sample_image*.jpg` – Example prediction images  
- `README.md` – Project documentation  

---

## 🛠 Requirements
- Python 3.8+
- Ultralytics YOLOv8

Install YOLOv8:
```bash
pip install ultralytics
```
---

## ▶️ Steps to Run

1. Install YOLOv8 using:
   pip install ultralytics

2. Place the images you want to test inside a folder (for example `test_images`).

3. From the project directory, run:
4. ```bash
   yolo task=detect mode=predict model=best.pt source=path/to/test_images/
   ```

5. The output images with bounding boxes will be saved in:
   ```bash
   runs/detect/predict/
   ```


