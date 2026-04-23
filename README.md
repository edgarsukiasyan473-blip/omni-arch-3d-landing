# Omni Arch — Immersive 3D Landing Experience

## Overview

**Omni Arch** is a high-end, single-page 3D landing experience that blends modern UI design with real-time WebGL rendering. Built with **Three.js** and **Tailwind CSS**, this project delivers a visually striking interface centered around a dynamic 3D object, atmospheric particles, and a glassmorphic content layer.

The goal of Omni Arch is to demonstrate how architecture, motion, and digital aesthetics can merge into a cohesive, immersive web experience—ideal for creative studios, experimental product launches, or next-generation portfolios.

---

## Features

* **Real-time 3D Rendering**

  * Interactive WebGL scene powered by Three.js
  * Animated torus knot centerpiece with physically-based material

* **Modern UI/UX Design**

  * Glassmorphism-based layout
  * Minimal, high-contrast typography
  * Responsive structure using Tailwind CSS

* **Ambient Motion System**

  * Subtle rotation animations
  * Particle field for depth and atmosphere
  * Smooth rendering loop optimized for performance

* **Single File Architecture**

  * Fully self-contained `index.html`
  * No build tools or installation required
  * Uses CDN-delivered dependencies

---

## Technologies Used

* **Three.js (r152)** — 3D rendering and animation
* **Tailwind CSS (CDN)** — Utility-first styling
* **Vanilla JavaScript** — Scene logic and animation control
* **WebGL** — Hardware-accelerated graphics

---

## Getting Started

### 1. Download or Clone

Simply place the `index.html` file into your project directory.

### 2. Run Locally

Open the file directly in your browser:

```bash
open index.html
```

Or use a lightweight local server (recommended):

```bash
npx serve
```

### 3. تجربه

Once opened, you’ll see:

* A floating 3D structure rendered in real time
* A centered hero panel with branding and call-to-action
* Subtle animated particles enhancing spatial depth

---

## Project Structure

```
/
└── index.html   # Complete application (UI + 3D + styling)
```

---

## Customization Guide

### Modify the 3D Object

Inside the script:

```js
const geometry = new THREE.TorusKnotGeometry(1, 0.3, 150, 20);
```

You can swap with:

* `BoxGeometry`
* `SphereGeometry`
* `IcosahedronGeometry`

---

### Adjust Colors & Theme

* Primary accent color:

```js
color: 0x6366f1
```

* Background gradient (CSS):

```css
background: radial-gradient(circle at 20% 20%, #0f172a, #020617);
```

---

### Control Animation Speed

```js
knot.rotation.x += 0.003;
knot.rotation.y += 0.005;
```

Lower values = smoother, slower motion
Higher values = more energetic feel

---

### Particle Density

```js
const particlesCount = 1000;
```

Increase for richer atmosphere, decrease for performance optimization.

---

## Performance Considerations

* Optimized for modern browsers with WebGL support
* Particle count and geometry complexity can be tuned for lower-end devices
* Uses requestAnimationFrame for efficient rendering cycles

---

## Use Cases

* Creative agency landing pages
* Experimental UI showcases
* Product launch microsites
* Portfolio intros for designers & developers
* Concept environments for immersive web design

---

## Future Enhancements

* Scroll-driven scene transitions
* Mouse interaction & parallax distortion
* Shader-based materials (neon, holographic effects)
* Multi-section storytelling layout
* WebGPU support (experimental)

---

## License

This project is open for personal and commercial use. Attribution is appreciated but not required.

---

## Author Note

Omni Arch is designed as a foundation for pushing the boundaries of web-based spatial design. It encourages experimentation—extend it, break it, evolve it.

---
