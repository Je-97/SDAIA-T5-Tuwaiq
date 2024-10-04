# RESD 
## (Real-Time Accident Detection and Classification for Enhanced Analysis)

_______________________________________________________________________________

## Overview
This project addresses the critical issue of traffic congestion in urban areas, which is often exacerbated by road accidents. The delay in emergency responses to accidents can further worsen the situation, increasing the severity of the congestion and putting more pressure on city infrastructure and emergency services. Our goal is to use AI-based solutions to mitigate these issues by providing real-time accident detection.

## Objective
In alignment with Vision 2030's emphasis on enhancing infrastructure and building smart cities, this project leverages computer vision to reduce traffic congestion and improve road safety. By implementing a state-of-the-art YOLOv8 object detection model on security cameras, we can quickly identify accidents and notify emergency services, resulting in faster response times and a safer urban environment.

## Solution Architecture
1. CCTV System: Security cameras in high-traffic areas capture live video streams.
2. Frame Extraction: Videos are converted into frames for further analysis.
3. Accident Detection: The YOLOv8 model detects accidents in Real-Time.
4. Classification: Detected accidents are classified as either "Accident" or "Severe Accident."
5. Notification: Emergency services are notified immediately in the case of severe accidents.


      ![image](https://github.com/user-attachments/assets/f786425b-e2bb-4179-be43-787755697fb4)


# Dataset
Source: 12,000 images from Roboflow, labeled into two classes: Accident and Severe Accident.
Additional Data: 461 images sourced from YouTube videos were added to enrich the dataset.
Preprocessing: Images were resized to 640x640, with noise and blur augmentation applied to enhance model generalization.

# Model & Result 
Model: YOLOv8
Training Configuration: 50 epochs, batch size of 16.
Performance Metrics:
Precision: 92%
Recall: 88%
mAP@0.5: 93%
   ![image](https://github.com/user-attachments/assets/2adf6868-1d9a-4e27-a4b4-b1e59930f782)

# Challenges
The primary challenge involved the dataset's complexity. Initially, the model misclassified large vehicles, like trucks, as accidents. We addressed this by adding more diverse images and creating a new class in the YAML configuration, improving the model's accuracy.
 ![image](https://github.com/user-attachments/assets/0aca61f5-6c29-483f-859f-2deef5cab99c)
 
# Demo



https://github.com/user-attachments/assets/c39f19da-5f78-4026-b865-3355fd9df104


# Future Work 
Adding more classes to capture different types of road incidents.
Deploying the model on dashcams in passing vehicles to further improve real-time response capabilities.
Diversifying the dataset to enhance performance in varying traffic conditions.

# Conclusion
This project demonstrates significant potential for improving road safety and reducing response times for accidents. By enabling faster identification and categorization of incidents, authorities can take swift action to manage traffic and ensure safer roads.

# Team Members
Jehan Almutairi

Haya Almalki

Hanan Mohammed



