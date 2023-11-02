# Vehicle Detection using OpenCV

## Overview
This project demonstrates a simple vehicle detection system using OpenCV, which can be used to detect vehicles in a video stream. It utilizes the Haar Cascade Classifier for car detection.

## Prerequisites
- Python
- OpenCV
- Installed Haar Cascade XML file (cars.xml)

## Getting Started
1. Clone the repository to your local machine.
2. Ensure you have Python and OpenCV installed.
3. Download the Haar Cascade XML file (cars.xml) from a trusted source.
4. Update the `cascade_src` variable in the code to the path of the cars.xml file.
5. Update the `video_src` variable to point to your video source (e.g., 'video2.avi' or '0' for a webcam).
6. Run the Python script using `python vehicle_detection.py`.

## Usage
- The script will open a video window displaying the detected vehicles in real-time.
- Press 'q' to quit the application.

## Customization
You can customize the parameters used for vehicle detection, such as the scale factor and minimum neighbors, by modifying the following line in the code:
```python
cars = car_cascade.detectMultiScale(gray, 1.1, 1)
