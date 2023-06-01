# Lane-Detection
This repository contains code for detecting and drawing lanes on road images or videos using OpenCV.
# Description
The 'main.py' file is the main script that performs lane detection on either an image or a video. It uses the following steps:

Convert the image to grayscale.
Apply Gaussian blur to reduce noise.
Apply Canny edge detection to detect edges in the image.
Define a region of interest to focus on the road area.
Use the Hough transform to detect lines in the region of interest.
Average and extrapolate the detected lines to estimate the lane boundaries.
Draw the estimated lane boundaries on the original image or video frame.
