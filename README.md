# 👕 AI Virtual Try-On Fitting Room

A browser-based virtual clothing try-on application that allows users to preview different outfits using their webcam. The application uses body-pose tracking and canvas-based clothing overlays to create an interactive virtual fitting-room experience.

## 📸 Project Preview

![AI Virtual Try-On Fitting Room](OutPut/Virtual%20Fit_%20Try%20On%20Your%20Style.png)

## 📖 Overview

The **AI Virtual Try-On Fitting Room** is designed to make clothing previews more interactive and accessible. Users can activate their webcam, select clothing items, and view clothing overlays positioned according to their body pose.

The project combines web development, computer vision, pose estimation, and real-time visual rendering to demonstrate a virtual clothing try-on workflow.

> **Note:** This project is a 2D clothing-overlay prototype. It does not provide photorealistic 3D garment simulation or physically accurate fabric fitting.

## ✨ Features

- 📷 **Live Camera Preview** — View yourself through your webcam.
- 🧍 **Body Pose Tracking** — Use pose landmarks to estimate body position when pose detection is enabled.
- 👕 **Multiple Clothing Options** — Preview available shirts, T-shirts, hoodies, jackets, and other supported outfits.
- 🎨 **Interactive Outfit Selection** — Switch between clothing options.
- 📐 **Body-Based Positioning** — Position clothing overlays using detected body landmarks.
- 🔄 **Camera Controls** — Use the available camera switching and reset controls.
- 📸 **Capture Preview** — Capture an image of the try-on preview if supported by the current implementation.
- 🌐 **Browser-Based Application** — Run the project in a compatible web browser.

## 🖼️ Screenshots

### 1. Hoodie Try-On

![Hoodie Try-On Screenshot](OutPut/Screenshot%202026-10-29%20213745.png)

### 2. T-Shirt Try-On

![T-Shirt Try-On Screenshot](OutPut/Screenshot%202026-10-29%20213819.png)

### 3. Full Outfit Preview

![Full Outfit Preview](OutPut/Screenshot%202026-10-29%20213840.png)

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Layout, styling, and responsive interface |
| JavaScript | Application logic and interactive controls |
| MediaPipe Pose | Body-pose estimation, if integrated in the application |
| HTML Canvas | Rendering clothing overlays and visual previews |
| Web Camera API | Accessing the user's camera |

*Verify the actual libraries and versions used in your source code before treating this list as a final dependency inventory.*

## ⚙️ How It Works

The application follows this general workflow:

1. The user opens the application in a web browser.
2. The user grants permission to access the webcam.
3. The application displays the live camera feed.
4. Pose estimation identifies relevant body landmarks, if enabled.
5. JavaScript uses the available landmarks to position and size clothing overlays.
6. The selected outfit is rendered over the camera preview.
7. The user switches outfits, resets the preview, or captures an image using the available controls.

### Architecture

```text
User
 |
 v
Web Interface (HTML + CSS)
 |
 v
JavaScript Application
 |
 +----------------------+
 |                      |
 v                      v
Webcam Feed        Clothing Selection
 |                      |
 v                      |
Pose Estimation         |
 |                      |
 v                      |
Body Landmarks          |
 |                      |
 +----------+-----------+
            |
            v
   Clothing Positioning
            |
            v
     Canvas Rendering
            |
            v
   Virtual Try-On Preview
            |
            v
       User Output
```

This diagram describes the intended workflow. Actual components depend on the implementation in the repository.

## 🚀 Getting Started

### Prerequisites

- A modern web browser such as Google Chrome or Microsoft Edge.
- A webcam for live try-on functionality.
- A code editor such as Visual Studio Code.
- An internet connection if the application loads libraries from external CDNs.

### Installation

**Step 1: Clone the repository**

```bash
git clone https://github.com/avinashreddy0/AI-Virtual-Try-On-Fitting-Room.git
```

**Step 2: Open the project folder**

```bash
cd AI-Virtual-Try-On-Fitting-Room
```

**Step 3: Open the project**

Open the folder in Visual Studio Code.

If the project uses only static HTML, CSS, and JavaScript, you can run it using the VS Code **Live Server** extension. Right-click `index.html` and select **Open with Live Server**.

Alternatively, use another local web server if required by your implementation.

**Step 4: Allow camera access**

Open the application through `localhost` or a secure HTTPS connection, grant camera permission, and test the available controls.

> If the application uses external libraries, make sure the browser can access those resources. Camera access may not work when the page is opened directly using a `file://` URL.

## 📂 Project Structure

```text
AI-Virtual-Try-On-Fitting-Room/
│
├── index.html
├── README.md
├── LICENSE
│
├── OutPut/
│   ├── Virtual Fit_ Try On Your Style.png
│   ├── Screenshot 2026-10-29 213745.png
│   ├── Screenshot 2026-10-29 213819.png
│   └── Screenshot 2026-10-29 213840.png
│
└── docs/
    ├── architecture.md
    ├── technical-report.md
    ├── third-party-components.md
    └── known-issues.md
```

*This structure assumes that the listed files and folders have been created and committed to the repository. Keep the structure in this README synchronized with the actual files.*

## 🧪 Testing

The application can be tested using the following checklist:

- [ ] The application loads without errors.
- [ ] Camera permission can be granted.
- [ ] The webcam preview displays correctly.
- [ ] Body-pose tracking works when enabled.
- [ ] Clothing options can be selected.
- [ ] Clothing overlays appear in the expected position.
- [ ] Camera switching works, if supported.
- [ ] Reset functionality works.
- [ ] Preview capture works, if supported.
- [ ] The interface remains usable at different screen sizes.

## ⚠️ Limitations

- The clothing preview is a 2D overlay rather than a complete 3D garment simulation.
- Clothing alignment may vary with body position, camera angle, lighting, and distance.
- Pose detection may be less reliable when body landmarks are obscured.
- Clothing overlays may not accurately represent garment size, draping, or fabric movement.
- Camera availability and performance depend on the user's browser and hardware.
- Actual fit, measurements, and clothing size cannot be guaranteed from the visual preview.

## 🔮 Future Enhancements

- Improve clothing alignment using more robust body-landmark tracking.
- Add support for more clothing categories and styles.
- Improve overlay scaling and positioning across different body shapes.
- Add more responsive layouts for mobile and desktop devices.
- Explore segmentation-based clothing overlays.
- Investigate 3D garment rendering and more realistic fabric simulation.
- Add optional user preferences and saved outfit selections.
- Improve accessibility, error handling, and browser compatibility.

## 🔐 Privacy

The application requests camera access for its live preview. Users should grant permission only when they intend to use the feature.

Do not assume that camera frames are processed exclusively on-device or never stored unless this has been verified in the implementation. Review the source code and any third-party services to confirm the application's actual data-handling behavior.

## 📚 Documentation

Additional project documentation, if included in the repository, is available in the `docs/` folder:

- [`Architecture`](docs/architecture.md)
- [`Technical Report`](docs/technical-report.md)
- [`Third-Party Components`](docs/third-party-components.md)
- [`Known Issues`](docs/known-issues.md)

## 👨‍💻 Author

**Avinash Reddy Induri**

- GitHub: [avinashreddy0](https://github.com/avinashreddy0)
- LinkedIn: [Avinash Reddy Induri](https://linkedin.com/in/avinash-reddy-induri-data-science/)

## 📄 License

This project is distributed under the MIT License. See the [`LICENSE`](LICENSE) file for details.

## 🙏 Acknowledgements

Thanks to the developers and maintainers of the web technologies and computer-vision libraries used in this project.

Please refer to the actual source code and third-party component documentation for the dependencies and applicable licenses.
