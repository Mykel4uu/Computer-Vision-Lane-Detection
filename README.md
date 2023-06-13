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
# Dependencies

1. Python 3
2. OpenCV
3. NumPy

# Usage

To use this code, follow these steps:

1. Clone the repository: ` git clone https://github.com/mykel4uu/lane-detection.git`
2. Install the required dependencies: `pip install opencv-python numpy`
3. Run the main.py script:
 For detecting lanes in an image, uncomment the following lines in the script: ```  image = cv2.imread('path/to/your/image.jpg')
lane_image = np.copy(image) ``` Replace 'path/to/your/image.jpg' with the actual path to your image file.
 For detecting lanes in a video, uncomment the following lines in the script: ``` cap = cv2.VideoCapture('path/to/your/video.mp4')
while(cap.isOpened()):
    _, frame = cap.read() ```
Replace 'path/to/your/video.mp4' with the actual path to your video file.  
4. Save the changes and run the script: ```python lane_detection.py```
The output will be displayed in a new window, showing the original image or video with the detected lanes drawn on it.

# Acknowledgments

The lane detection algorithm used in this project is based on the Hough transform technique.
Special thanks to the OpenCV and NumPy communities for providing the necessary tools and libraries.


