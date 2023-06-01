# Lane-Detection
This repository contains code for detecting and drawing lanes on road images or videos using OpenCV.
# Description
The main.py file is the main script that performs lane detection on either an image or a video. It uses the following steps:

1. Convert the image to grayscale.
2. Apply Gaussian blur to reduce noise.
3. Apply Canny edge detection to detect edges in the image.
4. Define a region of interest to focus on the road area.
5. Use the Hough transform to detect lines in the region of interest.
6. Average and extrapolate the detected lines to estimate the lane boundaries.
7. Draw the estimated lane boundaries on the original image or video frame.
