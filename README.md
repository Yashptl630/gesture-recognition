# Real-Time Body Language Detection with LSTM

This project uses the MediaPipe Holistic model and LSTM (Long Short-Term Memory) layers for real-time detection and prediction of body language signals from a person's face, hands, and pose.

## Project Description

The project uses OpenCV to capture video from the webcam. The video frames are processed using the MediaPipe Holistic model, which detects and returns the landmarks for the face, hands, and pose. These landmarks are then drawn onto the frames using MediaPipe's drawing utilities. The processed frames are displayed in real-time using OpenCV.

The landmarks data is then fed into an LSTM model for real-time prediction. The LSTM model is defined as follows:
This LSTM model consists of three LSTM layers followed by three Dense layers. The final Dense layer uses softmax activation and outputs the probabilities for 8 different classes.

Prerequisites
The project requires the following Python libraries:

OpenCV
MediaPipe
NumPy
Matplotlib
TensorFlow
