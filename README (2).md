Emotion Detector :
The Emotion Detector is an AI that utilizes imagenet to show human emotions from an image. This can be used in places like helping people who can’t show emotion as well express themselves and therapy.
![add image descrition here](direct image link here)

The Algorithm :
The algorithm uses imagenet to depict its confidence on what image is being shown. The AI was trained by a dataset from Kaggle based on thousands of pictures of people with different facial expressions such as neutral, sad, happy, angry, and surprised. 

Add an explanation of the algorithm and how it works. Make sure to include details about how the code works, what it depends on, and any other relevant info. Add images or other descriptions for your project here.


This video is a vitual demanstration of the AI working : https://youtu.be/ubG9VC_c8_U







## Datasets
The AI is trained using the datasets below with 50 epochs.


## Installation

install yolov8

```bash
  pip install ultralytics
```
If using YOLOv8 for live video (Classification):
```bash
  yolo task=classify mode=predict model=runs/classify/train/weights/best.pt source=0
```  
 If using YOLOv8 for pictures (Classification):
```bash
  yolo task=classify mode=predict model=runs/classify/train/weights/best.pt source=/home/nvidia05/Emotion_Detector/dataset/practice
```
Exporting to ONNX Type this command:
```bash
  yolo export model=runs/classify/train4/weights/best.pt format=onnx
```