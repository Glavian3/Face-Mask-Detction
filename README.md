# Real-time Face Mask Detection
This repository contains code for real-time face mask detection using the MobileNet model as the base model and OpenCV for image processing.

# Requirements
Python 3.x
OpenCV
Tensorflow
Numpy
You can install the required packages by running the following command:

```
pip install -r requirements.txt
```
# Usage
To run the code, use the following command:
```
python detect_mask_video.py
```
How it works
The MobileNet model is a lightweight deep neural network designed for mobile and embedded vision applications. It has a small memory footprint and low computational requirements, making it ideal for real-time face mask detection on low-power devices.

The pre-trained MobileNet model is used as the base model, with a few additional layers added on top for face mask detection. The model is trained on a dataset of images of people wearing and not wearing face masks.

During detection, the webcam feed is processed frame by frame. The face in each frame is detected using OpenCV's Haar Cascades classifier, and then passed through the MobileNet model for mask detection. The output of the model is then used to draw a bounding box around the face and label it as either "With Mask" or "Without Mask".
