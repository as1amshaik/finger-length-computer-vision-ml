# Finger Length Estimation from Hand Images

This project involves calculating the approximate length of each finger in a hand image using pixel intensity analysis. The input image is captured on a white background, making the hand region stand out with higher pixel values. Custom logic is used to detect fingers and measure their pixel length by scanning specific lines through the image.

## Project Overview

- Type: Image Processing / Computer Vision
- Goal: Estimate the length of each finger from a hand image
- Approach: Analyze pixel intensities along line scans from a predefined point
- Input: Hand image with a white background
- Output: Printed lengths of each finger and plotted intensity graphs

## Key Features

- Scans the hand image along fixed lines from a reference point
- Measures finger lengths based on continuous regions of high pixel intensity
- Plots intensity profiles to visualize finger detection
- Outputs estimated lengths in pixel units

## Algorithm Steps

1. Load the hand image in grayscale format.
2. Define a scanning origin (e.g., bottom center of the palm).
3. For each finger direction, define a line equation or scan angle.
4. Sample pixel values along the line.
5. Identify high-intensity regions that represent the finger.
6. Measure the pixel distance of each high-value segment (i.e., the length of the finger).
7. Plot pixel intensity vs. distance for visualization.
8. Print the estimated lengths.

## Skills Demonstrated

- Applied pixel-based analysis for feature detection
- Implemented line-based scanning using geometric constraints
- Used image profiles to infer shape-related metrics
- Visualized and interpreted raw image intensity data

## Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib

## How to Run

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install numpy opencv-python matplotlib
