# Car-and-pedestrian-tracking
This project is a Python-based application for detecting and tracking cars and pedestrians in videos using the OpenCV library. The program leverages pre-trained classifiers to identify objects of interest and visually highlights them with bounding boxes.

## Features
* Real-time detection and tracking of:
 * Cars
  * Pedestrians
* Highlights detected objects using colored rectangles:
  * Blue and Red: Cars
  * Yellow: Pedestrians
* Works with any video input that includes visible cars and pedestrians.
* Easy integration with custom datasets.

## Project Structure
### Main Files
* tracking.py: Core Python script for object detection and tracking.
* Supporting files for classifiers:
  * car_detector.xml: Pre-trained classifier for car detection.
  * haarcascade_fullbody.xml: Pre-trained classifier for pedestrian detection.

## Requirements
* Python 3.6 or above
* OpenCV library

## How It Works
1. Loads a pre-trained Haar Cascade classifier for car and pedestrian detection.
2. Reads video frames sequentially and converts them to grayscale for processing.
3. Detects objects using the classifiers and highlights them on the original video frames.
4. Displays the processed video with bounding boxes in a real-time window.

## Sample Output
The program highlights: 
* Cars with Blue/Red rectangles.
* Pedestrians with Yellow rectangles.

## Future Enhancements 
* Add support for real-time camera feeds.
* Integrate more advanced object detection models (e.g., YOLO or SSD).
* Improve detection accuracy and performance for edge cases.
