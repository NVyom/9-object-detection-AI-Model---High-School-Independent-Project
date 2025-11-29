#Object-detection-AI-Model---High-School-Independent-Project
Created a simple AI model to detect 9 food items, then implemented it on Raspberry Pi 5.

# Datasets Used
https://www.kaggle.com/datasets/raghavrpotdar/fresh-and-stale-images-of-fruits-and-vegetables
https://www.kaggle.com/datasets/anthonytherrien/image-classification-32-classes-food

# Project Overview
This project explores computer vision using a custom-trained CNN (Convolutional Neural Network) with data compiled from multiple open datasets.
The model detects 9 food items: apples, bananas, oranges, carrots, capsicum, rice, bitter gourd, broccoli, and tomatoes.
I deployed it on a Raspberry Pi 5 using its IMX219 camera for image inference, integrating eSpeak to audibly announce detected objects through connected headphones, accessibly designed for the visually impaired.

# Motivation
I developed this project for SANES (Saudi Arabia National Engineering & Science Fair/Symposium).
My aim was to explore AI’s role in accessibility and how a small, efficient device could aid people in areas with limited electricity or internet access.
This project also connected to my interest in Physics, as I wanted to understand how AI could be used in research contexts while also being used in the physical world in meaningful ways.

# Technical Details
All coded in Python.
Model is a MobileNetV2 backbone with transfer learning, which works best for lower power and efficient use.
Trained on a custom dataset of 9 classes (~500 images/class), with datasets from Kaggle.com.
Integrated with Picamera2 on Raspberry Pi 5 for inference (running the model to interact with the camera) and eSpeak for voice output.

# Challenges
I originally intended to develop a text detection system, but faced too many challenges with accuracy and implementation. It proved rather complex.
So I stuck with object detection, allowing me to refine my data handling and model design and training.
During training, my model accuracy plateaued due to a data leak, which I had trouble identifying. I resolved it after days of debugging, and in turn it deepened my understanding of data preprocessing and model validation.

# Uploaded Files
fruits.ipynb  -  My data pre-processing and AI model training file. I trained the model on my PC.

fruitdetect-Copy1.ipynb  -  My inference file, containing the code where I ran the AI model on my Raspberry Pi 5.

Nikhil's AI Project - Object Detection Examples.pdf - These are a few examples of accurate object detection done by my final model.

AI Project Science Fair Trifold.jpg - This is the trifold I prepared for the science fair I participated in (SANES).

AI Project - Raspberry Pi 5.jpg - This is the Raspberry Pi 5 I implemented my model on. Its camera and its case (for cooling and portability) are also included.

This experience strengthened my technical rigor, and I hope to hone these skills further to implement in future research projects.
