# 📺 Todd Hamilton CRT Display

A high-fidelity, interactive 3D CRT Monitor display inspired by Todd Hamilton's design. This project utilizes WebGL (Three.js) and custom GLSL shaders to recreate a nostalgic analog screen effect with modern interactions.

![Preview Placeholder](https://github.com/user-attachments/assets/92c151c6-d713-444a-90d8-04aa123eace6)


## ✨ Features

- **3D Environment:** A realistic project using Three.js to render a detailed CRT monitor model.
- **Dynamic Interactions:**
    - **Mouse Tracking:** The monitor rotates dynamically based on your mouse position.
    - **Hover Switching:** Hovering over project names instantly updates the monitor's display with smooth glitch transitions.
- **Analog Aesthetics:**
    - **CRT Shader:** Custom GLSL fragment shader simulating scanlines, chromatic aberration, and screen curvature.
    - **Glitch Effect:** Procedural glitch animation triggered during image transitions for an authentic "booting" feel.
- **Performance Optimized:** Built with Vite for lightning-fast development and optimized production builds.

## 🛠️ Technology Stack

- **Core:** [Three.js](https://threejs.org/) (WebGL)
- **Animation:** [GSAP](https://greensock.com/gsap/) (GreenSock Animation Platform)
- **Shaders:** GLSL (Custom Vertex & Fragment Shaders)
- **Models:** GLTF/GLB Loader
- **Build Tool:** [Vite](https://vitejs.dev/)
- **Languages:** JavaScript (ES6+), HTML5, CSS3

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Thakuma07/ToddHamilton-WEBGLAnimation.git
   cd todd-hamilton
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Run development server:**
   ```bash
   npm run dev
   ```

4. **Build for production:**
   ```bash
   npm run build
   ```

## 📂 Project Structure

```text
├── public/                 # Static assets (3D Models, Textures)
│   ├── monitor.glb         # Main 3D model
│   └── project-img-*.jpg   # Project screenshots
├── Shaders/                # GLSL Shaders
│   ├── fragmentShader.glsl # CRT and post-processing logic
│   └── vertexShader.glsl   # Screen geometry mapping
├── script.js               # Main Three.js setup and scene logic
├── styles.css              # Core layout and typography
├── index.html              # Entry point
└── package.json            # Dependencies and scripts
```

## 🎨 Customizing the Project

To add your own projects, simply update the `<ul>` list in `index.html`:

```html
<li data-img="/your-image.jpg">Project Name</li>
```

The `script.js` will automatically handle loading the new texture and applying the glitch effect on hover.

## 💎 Credits & Assets

- **Monitor Model:** Free 3D model sourced from [Sketchfab](https://skfb.ly/orHwK).
- **Model Optimization:** Cleaned and exported using the [Model Viewer Editor](https://modelviewer.dev/editor/).

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

Built with ❤️ by [thakuma.dev](https://github.com/Thakuma07)
