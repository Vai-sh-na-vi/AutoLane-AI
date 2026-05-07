# AutoLane AI – Intelligent Lane Tracking System

## Overview

AutoLane AI is an advanced computer vision based lane tracking framework developed for intelligent transportation and autonomous driving applications. The system is designed to detect, analyze, and visualize road lane boundaries from continuous video streams in real time.

By integrating multiple image processing and geometric transformation techniques, the project provides accurate lane estimation even in dynamically curved road environments.

The framework applies a sequence of optimized vision operations including edge extraction, perspective warping, histogram analysis, polynomial lane fitting, and sliding window tracking to identify lane structures with improved stability and precision.

The detected lane regions are projected back onto the original driving footage, enabling intuitive visualization for driver assistance systems and autonomous navigation research.

This project demonstrates how traditional computer vision algorithms can be combined efficiently to create a lightweight and reliable lane perception pipeline without requiring heavy deep learning models or GPU intensive computation.

---

# Key Features

## Real Time Lane Detection
Processes video frames continuously with low latency, enabling smooth and responsive lane tracking suitable for live driving simulations and autonomous vehicle prototypes.

## Perspective Bird’s Eye Transformation
Applies homographic perspective transformation to convert the front road view into a top down representation. This improves lane geometry interpretation and simplifies lane curvature estimation.

## Intelligent Sliding Window Search
Implements a histogram guided sliding window algorithm to identify lane pixels efficiently across curved and non linear road segments.

## Edge and Gradient Analysis
Utilizes advanced edge extraction methods based on Canny edge detection and gradient thresholding to isolate lane markings under varying illumination conditions.

## Polynomial Lane Curve Estimation
Fits detected lane pixels into smooth polynomial curves to generate stable lane trajectories and reduce detection noise between frames.

## Dynamic Lane Overlay Visualization
Projects the detected lane region back onto the original video feed with transparent highlighting for improved interpretability and visual feedback.

## Curved Lane Handling
Supports curved road tracking by continuously updating lane positions using adaptive search regions and pixel distribution analysis.

## Lightweight Architecture
Built entirely using classical computer vision techniques, making the system computationally efficient and suitable for systems with limited hardware resources.

---

# System Workflow

1. Video frames are extracted from the input driving footage.
2. Frames undergo preprocessing and color space normalization.
3. Edge features are extracted using gradient and threshold operations.
4. Perspective transformation converts the road into bird’s eye representation.
5. Histogram peaks are computed to locate initial lane positions.
6. Sliding windows scan vertically to identify lane pixels.
7. Polynomial regression estimates lane curvature.
8. Final lane boundaries are rendered on the original video frame.

---

# Technologies Used

- Python
- OpenCV
- NumPy
- MoviePy
- Matplotlib
- Jupyter Notebook / Google Colab

---

# Prerequisites

Before running the project, ensure the following dependencies are installed:

- Python 3.8 or higher
- OpenCV
- NumPy
- MoviePy
- Matplotlib
- Jupyter Notebook or Google Colab environment

---

