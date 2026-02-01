# Pole Detection using YOLOv8

This repository contains a YOLOv8 model trained to detect poles by color.

## Classes
- bluep
- redp
- yellowp

## Model
- Architecture: YOLOv8 Nano
- Trained on Roboflow Poles Dataset
- Checkpoint: best.pt

## How to Run Inference

```bash
yolo task=detect mode=predict model=best.pt source=path/to/images
