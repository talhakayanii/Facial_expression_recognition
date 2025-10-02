# Facial Expression Recognition-Deep Learning
This project implements a multimodal deep learning system for facial expression recognition using both image data and facial landmarks. The model predicts discrete expression categories (8 classes) and continuous valence-arousal values.

## Dataset
Download the dataset from: https://drive.google.com/file/d/1PdQBPUuHSBfEtK30cV2IIpRFBJ4-8B78/view?usp=sharing

The dataset contains facial images with corresponding .npy annotation files:

Expression labels (0-7): Neutral, Happy, Sad, Surprise, Fear, Disgust, Anger, Contempt

Valence values: Continuous from -1 (negative) to +1 (positive)

Arousal values: Continuous from -1 (tired) to +1 (active)

Facial landmarks: 68-point coordinates

## Model Architecture
Uses a multimodal approach with ResNet50 for image feature extraction and a fully connected network for landmark processing. Features are fused and passed to two output heads for expression classification (8 classes) and valence-arousal regression.
