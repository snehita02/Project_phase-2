# Object Detection for Visually Impaired People

## Introduction

Vision impairment is a significant global disability, affecting millions of people worldwide. Visually impaired individuals face numerous challenges in their daily lives, including difficulty identifying objects around them and navigating their surroundings. To address these challenges, we propose an object detection application that utilizes deep learning algorithms to assist visually impaired people in identifying objects and navigating their environment.

**Motivation**

Visually impaired individuals rely heavily on their sense of touch and hearing to navigate their surroundings and interact with the world around them. However, identifying objects and navigating complex environments can be challenging for visually impaired individuals using traditional methods. Object detection applications offer a promising solution to these challenges by providing real-time information about objects and their positions.

**Application Overview**

Our object detection application employs voice commands and deep learning algorithms to assist visually impaired people in identifying objects and navigating their surroundings. The application operates as follows:

1. **Voice Input:** The user provides voice commands to control the application and receive information.

2. **Speech Recognition:** A speech recognition library processes the user's voice commands and converts them into text.

3. **Object Detection:** The application utilizes a deep learning model, specifically a CNN (Convolutional Neural Network) architecture, to detect objects in real-time images captured from the device's camera.

4. **Image Segmentation and Recognition:** Image segmentation and image recognition techniques are employed to enhance the accuracy of object detection.

5. **Voice Output:** The application provides voice feedback, specifying the detected objects and their positions relative to the user.

## Benefits

Our object detection application offers several benefits to visually impaired individuals:

* **Enhanced Mobility and Navigation:** The application assists in identifying objects and navigating surroundings safely and independently.

* **Increased Confidence and Independence:** The ability to identify objects and navigate effectively empowers visually impaired individuals to perform daily tasks with greater confidence and self-reliance.

* **Improved Quality of Life:** The application can significantly enhance the quality of life for visually impaired individuals by providing them with greater independence and enabling them to participate more fully in everyday activities.

## Impact

The successful development and implementation of this object detection application can significantly improve the lives of visually impaired individuals by providing them with the ability to navigate their surroundings more effectively and identify objects of interest. This technology has the potential to enhance their daily activities, increase their independence, and improve their overall quality of life.

## Requirements

The following libraries and weights are required to run the application:

| Library/Weight | Version/Link |
|---|---|
| Python | 3.9.17 |
| NumPy | 1.24.3 |
| Keras | 2.13.1 |
| Keras-Preprocessing | 1.1.2 |
| opencv-python | 4.8.0.76 |
| pyttsx3 | 2.90 |
| SpeechRecognition | 3.10.0 |
| yolov3-416 weights | [Drive link](https://drive.google.com/file/d/1sRdGUSyfGW-tz-FaJ0-ufCjzVQF7sleX/view?usp=sharing) |

## Installation

To install the required libraries and weights, follow these steps:

1. **Install the libraries using the following commands:**

```bash
pip install python==3.9.17
pip install numpy==1.24.3
pip install keras==2.13.1
pip install keras-preprocessing==1.1.2
pip install opencv-python==4.8.0.76
pip install pyttsx3==2.90
```

2. **Download the yolov3-416 weights from the provided Drive link and place the downloaded file in the appropriate location within your project directory.**

## Usage

1. **Creating the Detection Model:**

Run yolo_algo.ipynb to create the YOLO object detection model. This will generate a model.h5 file.
The model only needs to be created once. The generated model.h5 can be reused.

2. **Running Object Detection:**

Run main.ipynb to run real-time object detection using the created model.h5.
main.ipynb needs to be executed each time you want to detect objects.
Connect a camera and point it at objects.
Detected objects and information will be conveyed through audio.
