# 🪨 Petroglyph Segmentation using YOLOv5 and OpenCV

This project focuses on segmenting petroglyphs (ancient rock carvings) using the YOLOv5 object detection model. The model is fine-tuned on a custom dataset to detect petroglyph regions in images.

## ⚙️ Environment Setup

Clone the YOLOv5 repository and install the necessary dependencies:
```
git clone https://github.com/ultralytics/yolov5
cd yolov5
pip install -r requirements.txt
pip install roboflow
```

## 🏋️ Finetune of model
To fine-tune a pretrained YOLOv5 model on the Petroglyph dataset:
```
python train.py \
  --weights {Path_to_model.pt} \
  --data {Path_to_data.yaml} \
  --cache
```