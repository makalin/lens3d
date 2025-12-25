# LENS3D 📸

![Platform](https://img.shields.io/badge/platform-macOS-black?style=for-the-badge&logo=apple)
![Swift](https://img.shields.io/badge/Swift-5.10-orange?style=for-the-badge&logo=swift)
![Metal](https://img.shields.io/badge/Render-Metal-blue?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

> **"The shutter closes. The dimension opens."**

**LENS3D** is a native macOS application that evolves photography into volumetric reality. It is a dedicated Gaussian Splatting studio with a "Deep Dark" interface, designed specifically for Apple Silicon to transform 2D photos into navigable 3D scenes.

![App Screenshot](./screenshot.png)

## 🌑 Features

### 1. The Obsidian Interface
A UI designed for focus. **LENS3D** features a custom pure-black (`#000000`) and slate-grey interface that recedes into the background, allowing your colorful point clouds to be the only source of light.

### 2. Single-Shot Splats
Experimental support for generative 3D.
* **Input:** A single `.jpg` or `.png`.
* **Process:** AI-driven depth estimation and geometry reconstruction.
* **Output:** A 360° explorable Gaussian Splat in seconds.

### 3. Studio Mode
For high-fidelity reconstruction:
* Drag and drop a folder of images or a video file.
* **LENS3D** handles the Colmap structure-from-motion (SfM) pipeline internally.

### 4. Metal-Powered Viewfinder
Built on a custom Metal backend to render millions of anisotropic gaussians at 60fps on M-series chips.

## 🛠 Tech Stack

* **UI Framework:** SwiftUI (macOS 14+)
* **Rendering:** Metal API (Custom Shader Pipeline)
* **Inference:** CoreML & PythonKit bridge
* **Architecture:** MVVM

## 🚀 Getting Started

### Prerequisites
* macOS Sonoma (14.0) or later
* Xcode 15+
* Apple Silicon (M1/M2/M3) highly recommended

### Installation

1.  Clone the repository:
    ```bash
    git clone [https://github.com/makalin/lens3d.git](https://github.com/makalin/lens3d.git)
    ```
2.  Navigate to the project directory:
    ```bash
    cd lens3d
    ```
3.  Open `LENS3D.xcodeproj` in Xcode.
4.  Build and Run (⌘R).

## 📸 Usage Workflow

1.  **Import:** Drag your source media into the "Aperture" drop zone.
2.  **Develop:** Click **"Process"**. The terminal log is hidden behind a sleek progress ring.
3.  **Inspect:** Use trackpad gestures to orbit, pan, and zoom into your splat.
4.  **Export:** Save as `.ply` or `.splat` for web usage.

## 🔮 Roadmap

- [ ] **LENS3D Cloud:** Offload heavy training to remote GPU clusters.
- [ ] **AR Preview:** Quick Look support for iOS/Vision Pro.
- [ ] **Post-Processing:** Crop and clean noise from splats directly in the app.

## 🤝 Contributing

Contributions are welcome. Please open an issue to discuss proposed changes or submit a Pull Request.

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

## 👨‍💻 Author

**Mehmet T. AKALIN**

* **Company:** [Digital Vision](https://dv.com.tr)
* **GitHub:** [@makalin](https://github.com/makalin)
* **LinkedIn:** [Mehmet T. AKALIN](https://www.linkedin.com/in/makalin/)
* **X (Twitter):** [@makalin](https://x.com/makalin)

---
*"Focus Beyond the Frame."*
