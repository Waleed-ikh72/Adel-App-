# Adel-App-
The SDAIA T5 Capstone project aims to improve traffic flow, reduce congestion, and enhance road safety in Saudi Arabia using advanced computer vision and machine learning techniques, aligning with Vision 2030. This project is made by Mohammed Al Malki, Mohammed Alrowais,Khaled AlGhamdi, and Waleed Al Ikhwan


![Project_logo](https://github.com/user-attachments/assets/d90faf4c-ee75-4157-a123-0f7eb6b1a56e)


# Traffic Solution Using Computer Vision

## Table of Contents
- [Overview](#overview)
- [Key Features](#key-features)
- [Methodology](#methodology)
  - [Traffic Density Model](#traffic-density-model)
  - [Violation Detection](#violation-detection)
- [Deployment](#deployment)
- [Results and Impact](#results-and-impact)
- [Future Work](#future-work)

## Overview
This project aims to develop a smart traffic signal system that measures vehicle density at each intersection, giving priority to the signal facing the highest traffic volume. This is achieved through the use of artificial intelligence technologies to analyze traffic data and determine the optimal time allocation for each signal based on the number of vehicles in each direction.

## Key Features

- **Vehicle Detection**: YOLOv8 detects vehicles in real time with high accuracy, categorizing vehicles like cars, trucks, buses, and motorbikes.
- **License Plate Recognition**: PaddleOCR is used for detecting and reading license plates, ensuring that violators are properly identified.
- **Traffic Signal Optimization**: The system dynamically adjusts traffic signal timing based on vehicle density at intersections, improving traffic flow.
- **Violation Detection**: Smart cameras monitor lane-crossing violations, with automatic notifications sent to violators, reducing manual law enforcement efforts.

## Methodology
- The system processes data collected from various sources, including:
  - Kaggle
  - Roboflow
  - Social media platforms
- The dataset includes annotated images of vehicles and license plates.
- Post-augmentation, the dataset contains over 1,900 images.
- YOLOv8 was used to train the models, achieving the following results:
  - Mean Average Precision (mAP) of 95% for vehicle detection.
  - Mean Average Precision (mAP) of 68% for license plates.

### Traffic Density Model
Using Roboflow, a model was trained to analyze vehicle density by categorizing cars, trucks, buses, and motorbikes. The model was fine-tuned to improve accuracy and optimize traffic signal allocation based on vehicle types and traffic levels at intersections.

### Violation Detection
We trained the YOLOv8n and YOLOv8s models to detect lane violations. The system also incorporates PaddleOCR for accurate license plate recognition. Violations are stored in an SQLite3 database, which maintains violator details, including vehicle images and license plate information.

## Deployment
The system is deployed using a **Streamlit app** on Hugging Face to leverage GPU processing for real-time traffic monitoring. Violators’ data is stored in SQLite3, and email notifications are sent regarding violations and associated fines.

## Results and Impact
- The model has achieved a high level of accuracy in:
  - Vehicle detection: 81%
  - Violation identification: 79%-91%
- The solution addresses traffic congestion and improves law enforcement efficiency.
- It supports the goals outlined in **Saudi Vision 2030**, contributing to:
  - Smarter urban transportation systems.
  - Safer road conditions.
## Libraries Used

1. streamlit
2. opencv-python
3. Pillow
4. numpy
5. moviepy
6. imageio[ffmpeg]
7. inference-sdk
8. ultralytics
9. deep_sort_realtime
10. imageio
11. paddlepaddle
12. paddleocr
13. matplotlib
14. pandas

## Contact
