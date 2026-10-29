# Known Issues and Future Improvements

## 1. Known Issues

The following are potential limitations of the current 2D overlay approach. Verify which issues occur in the running application.

### Clothing Alignment
Clothing overlays may become misaligned when detected landmarks are inaccurate or body movement is rapid.

### Pose Detection
Poor lighting, partial visibility, and camera positioning may affect landmark detection.

### 2D Garment Rendering
Canvas-based graphics cannot reproduce realistic fabric folds, wrinkles, or complete 3D garment movement.

### Body Occlusion
Arms and hands may not naturally appear in front of or behind the clothing overlay.

### Body Measurements
The prototype does not guarantee accurate body measurements or real-world garment sizing.

### Browser Compatibility
Camera behavior and performance can differ across browsers and devices.

### External Dependencies
Libraries or model assets loaded from external CDNs may require an internet connection.

## 2. Future Improvements

- Improve landmark smoothing and garment alignment.
- Add more accurate body segmentation and occlusion handling.
- Integrate a generative virtual try-on model.
- Support user-uploaded garment images.
- Improve mobile performance and responsive design.
- Add robust error handling for unavailable cameras.
- Add automated functional tests.
- Evaluate performance under different lighting conditions and poses.
- Add documented dependency versions and reproducible setup instructions.

## 3. Priorities

1. **High:** Verify camera access, outfit selection, and capture functionality.
2. **High:** Improve overlay alignment and error handling.
3. **Medium:** Improve mobile compatibility and automated testing.
4. **Future:** Explore generative garment replacement and more realistic fitting.