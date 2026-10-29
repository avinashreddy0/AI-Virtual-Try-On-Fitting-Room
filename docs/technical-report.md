# Technical Report — AI Virtual Try-On Fitting Room

## 1. Project Overview

Virtual Fit is a browser-based prototype that demonstrates virtual clothing visualization using computer vision and web technologies.

The application allows users to view a camera preview, select clothing designs, and visualize clothing overlays positioned relative to detected body landmarks.

## 2. Problem Statement

Online shoppers cannot physically try on clothing while browsing many online stores. This project explores how a webcam-based interface can provide a simple visual preview of different clothing styles.

## 3. Objectives

- Develop an interactive virtual fitting-room interface.
- Integrate browser camera input.
- Use pose estimation for body landmark detection.
- Render clothing overlays using HTML Canvas.
- Allow users to switch between available clothing designs.
- Explore the limitations of 2D virtual try-on.

## 4. Technologies

- HTML5 for application structure.
- CSS3 for styling and layout.
- JavaScript for application logic.
- HTML Canvas API for graphics rendering.
- MediaPipe Pose for body landmark detection, if configured in the source.
- Browser MediaDevices API for camera access, if used.
- Git and GitHub for source-code management.

## 5. Implementation

### User Interface

The interface provides camera preview and outfit selection controls.

### Camera Integration

The browser requests camera permission. Camera functionality depends on browser support, device availability, and permission settings.

### Pose Estimation

The pose-estimation component identifies body landmarks that can help determine approximate clothing placement.

### Clothing Rendering

JavaScript uses the available coordinates to position and scale clothing graphics. Canvas renders the resulting overlay.

### Preview Capture

The application provides capture functionality if implemented in the current source code.

## 6. Challenges

- Maintaining overlay alignment when the user moves.
- Handling inaccurate or missing pose landmarks.
- Managing different camera dimensions and screen sizes.
- Designing clothing graphics with suitable proportions.
- Handling camera permission errors and browser compatibility.

These are implementation challenges to validate against actual development and testing experience.

## 7. Testing and Validation

Test the following before submission:

- Application startup.
- Camera permission and initialization.
- Pose landmark detection.
- Clothing selection and overlay updates.
- Overlay alignment during movement.
- Camera switching, if implemented.
- Preview capture, if implemented.
- Layout on supported screen sizes.

Record the actual results, including failures. Do not report a test as passed unless it has been performed.

## 8. Limitations

- Clothing is represented by 2D graphics rather than complete 3D garments.
- Overlay alignment can be affected by pose-detection errors.
- Realistic fabric folds and physical movement are not simulated.
- Body occlusion may not always appear natural.
- The system does not guarantee actual garment size or fit.
- Performance depends on the device, browser, camera, and lighting.
- A generative virtual try-on model is not claimed as part of the current prototype unless one has been integrated.

## 9. Future Improvements

- Integrate a generative virtual try-on model.
- Improve garment alignment and body segmentation.
- Improve foreground and background occlusion.
- Add support for user-uploaded clothing images.
- Improve mobile responsiveness.
- Add automated tests and error handling.
- Evaluate performance across different devices and body poses.

## 10. Conclusion

Virtual Fit demonstrates a browser-based approach to clothing visualization through pose estimation and 2D graphics rendering. The project provides a foundation for further development of more realistic virtual try-on experiences.