# System Architecture — Virtual Fit

## 1. Overview

Virtual Fit is a browser-based virtual clothing visualization application. It uses camera input, pose estimation, JavaScript, and HTML Canvas to display clothing overlays.

## 2. Architecture Diagram

```text
User
  |
  v
Browser Interface (HTML + CSS + JavaScript)
  |
  v
Camera Input (Browser MediaDevices API)
  |
  v
MediaPipe Pose
  |
  v
Body Landmark Coordinates
  |
  v
Clothing Positioning and Scaling
  |
  v
HTML Canvas Overlay Rendering
  |
  v
Live Preview and Image Capture
```

## 3. Main Components

- **User Interface:** Displays the camera preview and outfit selection controls.
- **Camera Input:** Requests webcam access with the user's permission.
- **Pose Estimation:** Detects body landmarks using MediaPipe Pose, if configured in the application.
- **Landmark Processing:** Uses relevant coordinates to estimate clothing placement.
- **Canvas Rendering:** Draws clothing graphics over the camera preview.
- **Capture:** Produces an image of the preview if supported by the implementation.

## 4. Processing Workflow

1. The user opens the application.
2. The browser requests camera permission.
3. The application processes camera frames.
4. Pose estimation identifies relevant body landmarks.
5. JavaScript calculates approximate clothing positions.
6. Canvas renders the selected clothing overlay.
7. The user can select another outfit and capture the preview.

## 5. Architecture Limitations

The current design is a 2D overlay approach. It does not provide full 3D garment simulation, physically accurate fabric movement, or guaranteed real-world clothing fit.

The diagram should be updated if the implementation differs from this workflow.