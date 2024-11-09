VIRTUAL WHITEBOARD USING OpenCV
Ever dreamed of drawing in the air with just a wave of your finger? This project, "Virtual Whiteboard," allows you to sketch your imagination by tracking the movement of a colored marker with your camera. In this setup, a colored object placed at the tip of your finger serves as the marker.

We’ll utilize OpenCV’s computer vision techniques to bring this project to life. While Python is the recommended language due to its extensive libraries and user-friendly syntax, the fundamental concepts can be implemented in any language supported by OpenCV.

This project relies on color detection and tracking to achieve the desired outcome. The colored marker is identified, and a mask is created. This process involves subsequent morphological operations on the generated mask, specifically Erosion and Dilation. Erosion helps eliminate noise from the mask, and Dilation restores the eroded mask.

STEPS:
Capture Frames: Start by reading frames and convert them to the HSV color space (as it's easier for color detection).

Set Up Canvas: Prepare the canvas and add the necessary color buttons.

Adjust Trackbars: Fine-tune the trackbar values to find the mask of the colored marker.

Preprocess the Mask: Use morphological operations like Erosion and Dilation to refine the mask.

Detect Contours: Find contours, identify the center of the largest contour, and store these coordinates in an array for each frame (for drawing points on the canvas).

Draw on Canvas: Use the stored points to draw on the frames and canvas.

REQUIREMENTS:
Python 3

NumPy

OpenCV

By following these steps, you'll be able to create a Virtual Whiteboard that allows you to draw anything just by moving a colored marker in front of your camera.
