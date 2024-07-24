# 3D Rotating Donut ASCII Renderer in Go

## Overview

This Go program renders a rotating 3D donut (torus) using ASCII characters in the terminal.

## How It Works

1. **Initialization**:
    - Sets up two angles (`angleA` and `angleB`) for rotation.
    - Initializes depth and character buffers.

2. **Main Loop**:
    - Continuously resets the buffers.
    - Uses nested loops to calculate the 3D coordinates of points on a torus.
    - Projects these 3D points onto a 2D plane.
    - Updates the character buffer with appropriate ASCII characters based on the depth of each point.
    - Prints the character buffer to the terminal.

3. **Rotation**:
    - Increments `angleA` and `angleB` in each iteration to create a rotating effect.

## Running the Program

1. Save the code in a file named `donut.go`.
2. Run the program using:
    ```sh
    go run donut.go
    ```

## Key Concepts

- **3D to 2D Projection**: Converts 3D points to 2D for display.
- **Depth Buffer**: Keeps track of the depth of each point to render the correct ASCII character.
- **ASCII Characters**: Different characters represent different brightness levels, creating a 3D effect.

This program demonstrates the use of trigonometry and simple graphics techniques to create an animated 3D effect in a text-based environment.
