# color-detection-opencv
Mini project for detecting colors in an image using Opencv and mouse events
Overview:
This mini project demonstrates how to detect specific colors in an image by clicking on any pixel. It uses OpenCV's HSV color space and mouse event handling to dynamically create a mask and highlight the selected color region.

Features:
- Select any color by clicking on a pixel in the image
- Automatically calculates a range around the clicked HSV value
- Creates mask to isolate and display only the selected color
- Real time feedback through OpenCV windows
- Prevents overflow errors and ensures robust masking

Technologies used: python, OpenCV, NumPy

How it Works:
1. The image is converted from BGR to HSV color space.
2. A mouse callback function captures the HSV values of the clicked pixel.
3. A lower and upper bound is calculated around the HSV value.
4. A binary mask is created using cv2.inRange()
5. The original image is masked to highlight the selected color.

Future Improvements:
- Add trackbars to adjust HSV range manually
- Extend it to work on live webcam/video feed
- Detect and draw contours around masked objects
- Export HSV ranges for dataset creation or training
