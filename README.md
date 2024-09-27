# IMU-Video-Human-Action-Recognise
This repository is a multimodal human action recognise algorithm based on MoViNet and LSTM. 
# Dataset
The dataset for Human Action Recognition with IMUs and a Camera is provided at the following link:
https://drive.google.com/file/d/1tn91HX9y28Xy6x3cmq3V3b6SHgiwPRpx/view?usp=sharing
# Sliding Window
A sliding window of length 10 is used for Video and IMU data. They move forward in both the Video stream and the IMU data stream to ensure that the data fed into the model is synchronised and maintains the same length.
[Fig2_New13.pdf](https://github.com/user-attachments/files/17165224/Fig2_New13.pdf)
# Model
A new multimodal human action recognition model is proposed, which uses MoVinet to process the video data and LSTM to extract features from the IMU data, and finally fuses the above two features to classify the three actions of grasping, walking and placing during the process of carrying a box.
[Fig4.pdf](https://github.com/user-attachments/files/17165299/Fig4.pdf)
# Start
  pip install -r requirements.txt
  python train_eval.py
