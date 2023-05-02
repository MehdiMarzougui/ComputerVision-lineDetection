# ComputerVision-lineDetection

This repository contains a Python implementation of a basic lane detection algorithm. The program processes a video file and returns a version of the video with detected lane lines highlighted.

## Requirements

- Python 3.6+
- OpenCV

## Usage

1. Place the input video file (e.g., `test.mp4`) in the project directory.

2. Run the lane detection script: lanes.py

3. Press the "a" key to stop the video and exit the program.

## Algorithm

The lane detection algorithm consists of the following steps:

1. Convert the input frame to grayscale.
2. Apply Gaussian blur to reduce noise.
3. Perform edge detection using the Canny algorithm.
4. Define a region of interest to focus on the road.
5. Detect lines using the Hough transform.
6. Separate lines into left and right lanes based on their slope.
7. Calculate the average slope and intercept for each lane.
8. Extrapolate the lane lines and overlay them on the original frame.
