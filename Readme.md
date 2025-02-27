Vehicle Counting and Speed Estimation Using YOLOv8
=================================================

This project leverages the cutting-edge capabilities of YOLOv8 for real-time vehicle counting and speed estimation. It is designed to aid in traffic monitoring systems, enhancing road safety and traffic management.

## ⚠ Disclaimer
This tool is developed for educational and developmental purposes. It's crucial to understand the implications and responsibilities of using such technologies in real-world applications.

## Project Overview

*Example image showing detected vehicles and their tracking.*

![Image](image0.jpg)

### After :rocket: :car: :dash:


![After](after.png)

## How to Use

1. **Prepare Your Environment**:
    Ensure you have Python, OpenCV, and the ultralytics YOLO library installed.

2. **Clone the Repository**:
    ```sh
    git clone https://github.com/yourgithub/vehicle-detection-yolov8.git
    ```

3. **Run the Detection**:
    Navigate to the cloned directory and run:
    ```sh
    python main.py
    ```

## How it Works

The script processes video frames to detect and track vehicles using YOLOv8. It then counts these vehicles as they cross a predefined line in the video, effectively estimating the flow of traffic.

- **Initialization**: Load the YOLOv8 model and start capturing video from a file.
- **Detection**: The model predicts vehicles in each frame and outputs their bounding boxes.
- **Tracking**: Custom tracking logic updates the trajectory of each detected vehicle.
- **Counting**: Vehicles crossing a predefined line are counted and the total is displayed on the output video.

## Customizations

You can adjust several parameters including the video source file, the sensitivity of the detection, and the specifics of the tracking algorithm.

For example, to change the video source:
```sh
python main.py --video_path=new_video.mp4
```

## System Requirements
- **Python 3.x**
- **OpenCV library**
- **Ultralytics**
- **YOLO library

## Troubleshooting
No detections in the video
Ensure your model file is correctly loaded and the video file path is correct. Check if the video has clear visibility and minimal occlusions.

## Tracking issues
Adjust the tracking parameters if the vehicles are not being consistently followed across frames.

## Performance is slow
Try reducing the video resolution or using a more powerful GPU. YOLOv8 is resource-intensive.

## Still need help?
Open an issue on our GitHub repository, and we will help you as soon as possible.

Enjoy exploring and extending this project! Feel free to contribute and suggest improvements.
