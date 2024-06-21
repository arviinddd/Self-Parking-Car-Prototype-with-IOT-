# Self-Parking-Car-Prototype-With-IOT

Parking a 4-wheeler can be a daunting and noisy task, especially in areas where parking space is limited. The process often involves multiple forward and backward maneuvers and turns, which can be challenging for many drivers, particularly those new to driving. In response to this challenge, our project introduces an autonomous self-parking system designed to navigate and park in specific spaces autonomously. This system uses a combination of proximity sensors to identify suitable parking spots and execute parking maneuvers seamlessly.

# System Overview
The autonomous parking system is designed to autonomously steer a vehicle into identified parking spots, handling both parallel and perpendicular parking scenarios. The system features an integrated approach that combines parking space searching, vacant space detection, and precise steering control. The technology stack includes:

Speed Sensor (LM393): Manages the vehicle's speed during parking to ensure safety and precision.
Ultrasonic Sensor: Scans the parking environment to detect empty spaces, providing real-time data for parking maneuvers.
ESP32-CAM Module: Facilitates connection to the IoT Cloud, enabling remote access and control of the prototype through the internet. This module also captures real-time images that are processed for object detection and space assessment.
# Key Functionalities
Parking Space Detection: Utilizes ultrasonic sensors to identify available parking slots. The system evaluates the dimensions of the space to determine if it fits the vehicle's requirements for either parallel or perpendicular parking.
Image Processing: Implements OpenCV on a Raspberry Pi 3 Model B+ to process images captured by the ESP32-Cam. The system uses Haar Cascades for dynamic object detection and Homography for precise mapping of the parking area.
Autonomous Steering Control: Based on the data from sensors and image processing, the vehicle executes calculated parking maneuvers, adjusting its position with sophisticated steering algorithms.
Remote Monitoring and Control: Integrates with the Arduino IoT Cloud to offer a user-friendly dashboard interface. This allows users to monitor the parking process in real time and intervene if necessary, enhancing the usability and safety of the autonomous parking system.
# Implementation and Testing
The prototype is rigorously tested to ensure robust performance across different parking environments. Integration testing confirms the seamless operation of sensors, processing units, and control mechanisms. Functionality tests are conducted in various lighting and space conditions to validate the reliability of the parking algorithms and sensor accuracy.
