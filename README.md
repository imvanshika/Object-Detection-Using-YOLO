# Indoor Object Detection Using YOLOv8

This project demonstrates the application of the YOLOv8 (You Only Look Once) model for detecting objects in indoor environments. The model is trained to recognize a variety of common objects typically found indoors, providing real-time object detection with high accuracy.

## Table of Contents
- Project Overview
- Features
- Installation
- Dataset
- Training
- Model
- Results
- Contributing

## Project Overview
Indoor object detection is a vital part of many applications such as home automation, surveillance, and robotic navigation. This project uses the latest YOLOv8 model to detect objects in real-time from indoor environments. The trained model can identify objects such as chairs, tables, monitors, laptops, and other household or office items.

## Features
- Real-time indoor object detection.
- Utilizes the YOLOv8 architecture for fast and accurate predictions.
- Pre-trained model on a custom indoor object dataset.
- Python implementation using the Ultralytics YOLOv8 library.
  
## Installation


1. **Clone the repository**:
   ```bash
   
   git clone https://github.com/yourusername/indoor-object-detection-yolov8.git
   cd indoor-object-detection-yolov8
2. **Install the requirements**:
   ```bash
      pip install -r requirements.txt
   
The main dependencies include:

  ultralytics (for YOLOv8)
  opencv-python
  matplotlib
  Dataset
The dataset used for training the YOLOv8 model consists of indoor objects such as chairs, tables, couches, monitors, and other commonly found items in homes and offices. The dataset was annotated using Roboflow for bounding box detection. You can find dataset in this repository.

## Training
To train the YOLOv8 model on your own dataset:

Prepare your dataset with annotations in YOLO format.
Train the model using the following command:

```
    python train.py --data data.yaml --weights yolov8n.pt --epochs 100 --img 640
```

Adjust epochs and img size as per your requirements.

## Model
The model was trained using the YOLOv8 architecture. YOLOv8 is a state-of-the-art object detection model that offers higher accuracy and faster inference compared to its predecessors. The following YOLOv8 versions were used:

YOLOv8n (nano version) for faster real-time detection with lower computational resources.
Pre-trained weights are available in the weights folder or can be downloaded from Ultralytics Hub.
## Results
Here are some sample results from the model:

Image 1

Image 2

The model achieved a high accuracy in detecting common indoor objects with a mAP of 85% on the validation set.

## Contributing
Feel free to contribute by submitting issues, pull requests, or any other feedback!

## Fork the repository.
Create a new branch for your feature or bug fix.
Submit a pull request with a clear description of your changes.
