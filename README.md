# 👕 AI Virtual Try-On Fitting Room | Virtual Fit

## 🖼️ Project Thumbnail

<p align="center">
  <img src="OutPut/Virtual%20Fit_%20Try%20On%20Your%20Style.png"
       alt="Virtual Fit — AI Virtual Try-On Fitting Room"
       width="100%"/>
</p>

<h3 align="center">✨ Try On Your Style. Virtually.</h3>

<p align="center">
  👕 Virtual Outfits · 🧍 Pose Detection · 📷 Live Camera · 📸 Capture Your Look
</p>
---

## 📌 About the Project

**AI Virtual Try-On Fitting Room — Virtual Fit** is a browser-based application designed to demonstrate virtual clothing try-on using computer vision and web technologies.

The application uses **MediaPipe Pose** to detect body landmarks and **HTML Canvas** to render virtual clothing overlays on the live camera feed. Users can select different outfits, preview clothing styles, switch cameras on supported devices, and capture their virtual look.

The project focuses on creating an interactive virtual fitting-room experience without requiring users to physically change clothes.

## 🎯 Project Objectives

- 👕 Allow users to preview different clothing styles virtually.
- 📷 Display a real-time webcam feed.
- 🧍 Track body landmarks using MediaPipe Pose.
- 🎨 Render clothing overlays using HTML Canvas.
- 👖 Provide different outfit combinations.
- 🔄 Allow users to switch between available outfits.
- 📸 Capture and download the virtual try-on preview.
- 📱 Provide a clean and interactive user interface.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 📷 Live Camera | Displays the user's webcam feed. |
| 🧍 Pose Detection | Detects body landmarks using MediaPipe Pose. |
| 👕 Outfit Selection | Allows users to select different clothing designs. |
| 🎨 Clothing Overlays | Draws virtual garments using canvas shapes and colors. |
| 🧥 Hoodie Designs | Includes hood shapes, face openings, and drawstrings for selected hoodies. |
| 👖 Outfit Combinations | Supports selected combinations of tops, pants, shorts, and tracksuits. |
| 🎭 Clothing Details | Adds selected stripes, buttons, lapels, pockets, and other design details. |
| 🔄 Camera Switch | Switches cameras where supported by the browser and device. |
| ♻️ Reset Option | Resets the current outfit selection. |
| 📸 Capture Look | Captures the current preview as a downloadable image. |
| 📱 Responsive Interface | Provides an interface designed for different screen sizes. |

---

## 👗 Available Outfit Collection

The application includes the following outfit designs.

### 👕 T-Shirts and Casual Wear

- ⚫ Black Tee
- 🌸 Pink Boxy Tee
- 🔴 Red Graphic Tee
- 🟡 Yellow Sport Tee
- 🟣 Purple Oversized Tee
- ⚪ Striped Tee

### 🧥 Hoodies and Sweatshirts

- 🤍 Cream Hoodie
- 🫒 Olive Hoodie
- ⚫ Black Hoodie + Cargo
- 🍷 Maroon Hoodie + Joggers
- 🤍 Cream Sweatshirt

### 👔 Shirts, Jackets and Formal Wear

- 🔵 Blue Oxford Shirt
- 🧥 Denim Jacket + Jeans
- 🤍 White Shirt + Formal
- 🕴️ Suit + Trousers

### 👖 Complete Outfit Combinations

- 👖 White Tee + Jeans
- ⚫ Grey Tee + Black Jeans
- 🟠 Orange Tee + Cargo
- 🟢 Green Tee + Shorts
- 🌿 Mint Tee + Chinos
- 🔵 Blue Tee + Joggers
- 🌌 Navy Tracksuit
- ⚫ All-Black Outfit

*Note: The list represents the intended outfit collection. The exact outfits available depend on the current application code.*

---

## 🖥️ Application Screenshots

### 🫒 1. Olive Hoodie

<p align="center">
  <img src="OutPut/Screenshot 2026-10-29 213745.png" alt="Virtual Fit — Olive Hoodie Preview" width="650"/>
</p>

Preview the olive hoodie design, including the hood opening, drawstrings, and torso overlay.

### 🌸 2. Pink Boxy Tee

<p align="center">
  <img src="OutPut/Screenshot 2026-10-29 213819.png" alt="Virtual Fit — Pink Boxy Tee Preview" width="650"/>
</p>

Preview a pink boxy T-shirt with a colored torso overlay and sleeve shapes.

### ⚫ 3. All-Black Outfit

<p align="center">
  <img src="OutPut/Screenshot 2026-10-29 213840.png" alt="Virtual Fit — All-Black Outfit Preview" width="650"/>
</p>

Preview the all-black outfit design using the live camera and virtual clothing overlays.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🌐 HTML5 | Defines the application structure. |
| 🎨 CSS3 | Handles styling, layout, and responsive design. |
| ⚙️ JavaScript | Implements application logic and interactions. |
| 🖌️ HTML Canvas API | Draws clothing overlays and creates captured images. |
| 🧍 MediaPipe Pose | Detects body landmarks in the camera feed. |
| 📷 WebRTC Camera API | Accesses the webcam through the browser. |
| 📦 jsDelivr CDN | Loads external libraries when configured in the application. |

---

## 🧠 How the Application Works

The application follows a real-time processing workflow.

1. **📷 Camera Initialization:** The browser requests permission to access the webcam.
2. **🧍 Pose Detection:** MediaPipe Pose detects body landmarks from camera frames.
3. **📍 Landmark Extraction:** Relevant body coordinates are identified.
4. **📐 Position Calculation:** Landmark positions help determine where clothing overlays should be drawn.
5. **🎨 Clothing Rendering:** Canvas shapes are drawn around selected body regions.
6. **👕 Outfit Selection:** Users can change the clothing design using the outfit carousel.
7. **📸 Image Capture:** The current camera preview and clothing overlay are combined into a captured image.

### 🔄 Application Workflow

```text
           📷 Webcam Feed
                 |
                 v
       🧍 MediaPipe Pose
                 |
                 v
      📍 Body Landmark Detection
                 |
                 v
       📐 Position Calculation
                 |
                 v
       🎨 Canvas Clothing Overlay
                 |
                 v
        👕 Select Different Outfit
                 |
                 v
       🖥️ Live Virtual Try-On
                 |
                 v
          📸 Capture Look
```

---

## 📂 Project Structure

```text
AI-Virtual-Try-On-Fitting-Room/
│
├── index.html
├── README.md
│
├── OutPut/
│   ├── virtual-fit-thumbnail.png
│   ├── Screenshot 2026-10-29 213745.png
│   ├── Screenshot 2026-10-29 213819.png
│   └── Screenshot 2026-10-29 213840.png
│
└── LICENSE
```

**Folder descriptions:**

- `index.html` — Main application file, if your current code is contained in a single HTML file.
- `README.md` — Project documentation.
- `OutPut/` — Project thumbnail and application screenshots.
- `LICENSE` — Optional license file to add when you choose your project's distribution terms.

---

## 🚀 Getting Started

Follow these steps to run the application locally.

### 1️⃣ Prerequisites

Make sure you have:

- 💻 A computer with a modern web browser.
- 📷 A working webcam.
- 🌐 An internet connection if the application loads MediaPipe or other libraries from a CDN.
- 🐍 Python installed, if you want to use Python's built-in local web server.

### 2️⃣ Open Your Project Folder

Navigate to the project directory:

```text
C:\Users\indur\OneDrive\Desktop\Ass\AI-Virtual-Try-On-Fitting-Room
```

### 3️⃣ Start a Local Web Server

Open a terminal in the project folder and run:

```bash
python -m http.server 8000
```

Alternatively, on Windows:

```bash
py -m http.server 8000
```

### 4️⃣ Open the Application

Open your browser and visit:

```text
http://localhost:8000
```

Make sure your main HTML file is named `index.html` and is located in the directory being served.

### 5️⃣ Allow Camera Access

When the browser asks for camera permission, click **Allow**.

The application should then be able to access the camera, subject to browser permissions and device support.

---

## 📸 How to Use Virtual Fit

1. 🌐 Open the application in your browser.
2. 📷 Allow webcam access.
3. 🧍 Stand in front of the camera so your body is visible.
4. 👕 Select a clothing item from the outfit carousel.
5. 🎨 Preview the selected clothing overlay.
6. 🔄 Switch cameras if the feature is supported and needed.
7. ♻️ Use Reset to return to the default selection.
8. 📸 Click **Capture Look** to download the current preview.

💡 **Tip:** Good lighting, a visible upper body, and a clear camera view can improve pose detection and overlay alignment.

---

## 📸 Capturing Your Look

The capture feature is designed to save the current virtual try-on preview as an image.

The captured result may include:

- 📷 The camera frame.
- 👕 The selected clothing overlay.
- 🎨 The rendered clothing colors and details.

The final result depends on the capture implementation in the current application code.

---

## ⚠️ Current Limitations

Virtual Fit is a **2D virtual clothing overlay prototype**, rather than a fully photorealistic AI garment replacement system.

- 🎭 **2D garment rendering:** Clothing is drawn with canvas shapes, so it may look flat rather than like real fabric.
- 🧍 **Pose accuracy:** Overlays can become misaligned if body landmarks are detected incorrectly or hidden.
- 🧵 **Fabric simulation:** Realistic folds, wrinkles, and cloth movement are not simulated.
- 🔄 **Front and back views:** The application does not provide complete 3D garment wrapping or automatic front-to-back garment simulation.
- ✂️ **Body occlusion:** Arms, hands, and other body parts may not always appear in front of or behind clothing naturally.
- 📏 **Size accuracy:** The overlay does not determine actual clothing measurements or guarantee a real-world fit.
- 📱 **Performance:** Tracking quality and frame rate depend on the device, browser, and camera.

These limitations are expected for a canvas-based prototype and can be addressed in future versions.

---

## 🔮 Future Improvements

Potential enhancements include:

- 🧠 Integrate an AI virtual try-on model for more realistic clothing replacement.
- 🧵 Use garment images or 3D clothing assets instead of simple shapes.
- ✂️ Add body segmentation for more accurate foreground and background layering.
- 📐 Improve garment scaling and alignment based on body measurements.
- 🔄 Improve tracking when users rotate or move their bodies.
- 👗 Allow users to upload their own clothing images.
- 🪞 Add a more realistic virtual mirror interface.
- 💾 Add saved outfits and try-on history.
- 📱 Improve mobile compatibility and performance.
- 🧪 Add automated tests and more robust error handling.

---

## 🔐 Privacy

- 📷 Camera access requires permission from the user.
- 🔒 Camera permissions are controlled by the browser.
- 💾 Captured images can be saved locally through the browser's download feature.
- 🌐 External libraries may be loaded from a CDN.

The application is not intended to upload webcam footage or captured images to a backend. Verify the actual code and any external dependencies before making stronger privacy claims.

---

## 🎓 Learning Outcomes

This project provides practical experience with:

- 🧠 Computer vision and pose estimation.
- 🧍 Body-landmark detection.
- ⚙️ JavaScript application development.
- 🎨 Canvas-based graphics rendering.
- 📷 Browser camera integration.
- 📐 Coordinate mapping and garment positioning.
- 🖥️ Interactive and responsive user interfaces.
- 🛠️ Debugging real-time visual applications.

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. 🍴 Fork the repository.
2. 🌿 Create a new branch for your changes.
3. 💻 Implement and test your improvements.
4. 📦 Commit your changes with a clear message.
5. 🚀 Submit a pull request.

---

## 📄 License

This project does not have a specified license in this README yet.

Choose an appropriate open-source license and add its corresponding `LICENSE` file before publishing the project for reuse.

---

## 👨‍💻 Author

**Avinash Reddy**

- 💼 LinkedIn: [Connect on LinkedIn](https://linkedin.com/in/avinash-reddy-induri-data-science/)
- 🐙 GitHub: [Visit GitHub](https://github.com/avinashreddy0)

---

<p align="center">
  👕 <strong>Virtual Fit — Explore Your Style, Virtually.</strong> ✨
</p>

<p align="center">
  Built with ❤️ using JavaScript, HTML Canvas, and MediaPipe Pose.
</p>
