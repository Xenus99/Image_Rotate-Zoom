# Image Transformation and Display (Java)

## Overview
This project is a Java application that takes an RGB file as input and performs image transformations such as rotation and zooming, displaying the output as a continuous video-like stream. The image rotates and zooms based on user-defined parameters, with real-time rendering through pixel-by-pixel transformation.

## Features
- Rotate images clockwise or anti-clockwise.
- Zoom in or out with customizable scaling factors.
- Real-time transformation at specified frames per second (FPS).

## Usage
To run the program, use the following command in the terminal:

```bash
java ImageDisplay.java FILEPATH ZOOMING_FACTOR ROTATION_FACTOR FPS
```

## Parameters:
- **FILEPATH:** Path to the RGB image file.
- **ZOOMING_FACTOR:** Zoom scaling factor (0.5 for half size, 2 for double size, etc.).
- **ROTATION_FACTOR:** Rotation speed and direction (- for anti-clockwise, + for clockwise).
- **FPS:** Frames per second (higher values create smoother transformations).

## Example:
```bash
java ImageDisplay.java image.rgb 1.5 45 30
```
This example rotates the image at 45 degrees per second, zooms in by 1.5x, and displays 30 frames per second.

## Requirements
- Java Development Kit (JDK) 1.8 or higher.
  
## How it Works
The application performs pixel-by-pixel transformation using a mathematical function that recalculates each pixel's new position on the canvas. The transformations are applied in real time to simulate continuous motion.
