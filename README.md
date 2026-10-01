# ✨ Interactive Birthday Celebration Web Experience

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Anime.js](https://img.shields.io/badge/Anime.js-FF4E83?style=for-the-badge&logo=javascript&logoColor=white)](https://animejs.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

An immersive, multi-stage interactive birthday greeting web application engineered with modern web technologies, fluid 60 FPS animations, realistic physics-inspired interactions, and responsive glassmorphic aesthetics.

---

## 🌟 Overview

This web experience transforms a traditional birthday greeting into an unforgettable, gamified visual journey. From the initial mystery gift box to an interactive candle blow-out, Polaroid memory gallery, scratch-off vouchers, and a grand finale celebration with floating atmospheric balloons and fireworks, every element is designed to spark joy and excitement.

---

## ✨ Features Breakdown

### 🎁 1. Interactive Surprise Gift Box
- **Engaging Entrance**: Pulsing 3D gift box with synchronized ambient heartbeat glow.
- **Micro-Interaction**: Click or tap to launch an animated lid opening transition.
- **Audio Initialization**: Seamlessly initializes celebration background music on first user gesture.

### 💌 2. Heart Envelope & Typewriter Letter
- **SVG Path Animation**: Mathematical parametric heart curve traced in real-time.
- **Emotional Typewriter**: Natural cadence typewriter effect with adaptive punctuation pauses.
- **Ambient Magic Dust**: Sparkling particle dust generator orbiting the letter scene.

### 🎂 3. 3D Cake & Candle Blow-out
- **High-Definition Visuals**: Centered custom 3D celebration birthday cake.
- **Interactive Flame**: Animated glowing flame with natural flickering physics.
- **Interactive Blow-out**: Click or tap the candle flame to blow it out with a realistic smoke effect and milestone toast celebration.

### 📸 4. Polaroid Memory Showcase
- **Glassmorphic Card Deck**: Real-time perspective transforms on hover and touch.
- **Curated Memories**: High-resolution photo moments with heartfelt customizable captions.
- **Responsive Stacking**: Seamlessly scales across desktop, tablet, and mobile displays.

### 🎟️ 5. Interactive VIP Scratch-off Vouchers
- **HTML5 Canvas Scratcher**: Custom coin cursor and realistic scratch-reveal mechanic.
- **Smart Threshold Engine**: Automatically unlocks with a celebration sparkle once 70% of the surface is scratched.
- **Customizable Rewards**: Tailor vouchers for personalized surprise gifts (e.g., Dinner Date, Endless Hugs, Shopping Spree).

### 🎆 6. Grand Finale & Audio Control
- **Full-Sky Atmospheric Balloons**: 5-zone balanced balloon algorithm guaranteeing even distribution across left, center, and right viewport boundaries.
- **Confetti Cannons**: Dynamic particle bursts celebrating key stage transitions.
- **Floating Audio Controller**: Sleek floating glassmorphism player with real-time toggle controls.

---

## 📂 Project Structure

```
happybirthday/
├── image/
│   ├── b3.png               # Decorative floral corner accent
│   ├── b4.png               # Decorative floral corner accent
│   ├── b5.png               # Floating heart element
│   ├── b6.png               # Floating heart element
│   ├── bg.png               # Primary celebration backdrop
│   ├── cake_3d.png          # 3D Birthday Cake asset
│   ├── giftbox.png          # Decorative gift box illustration
│   ├── hop.png              # Interactive gift box base
│   ├── nap.png              # Interactive gift box lid
│   ├── heartAnimation.gif   # Dynamic heart animation asset
│   ├── mewmew.gif           # Cute celebratory character animation
│   ├── photo_cake.jpg       # Memory gallery photo asset
│   └── photo_roses.jpg      # Memory gallery photo asset
├── flower.jpg               # Memory showcase visual
├── image.jpg                # Memory showcase visual
├── happybirthday.mp3        # Celebration background music track
├── index.html               # Main application entry point & logic
└── README.md                # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites
- Any modern web browser (Google Chrome, Mozilla Firefox, Safari, Microsoft Edge, Opera).

### Local Execution
1. Clone or download this repository to your local machine:
   ```bash
   git clone https://github.com/your-username/interactive-birthday-celebration.git
   ```
2. Navigate to the project directory:
   ```bash
   cd interactive-birthday-celebration
   ```
3. Open `index.html` directly in your browser:
   - **Double-click** `index.html`, OR
   - Run a local development server (e.g., using VS Code Live Server or `npx serve .`).

---

## 🛠️ Customization Guide

### 1. Modifying Text & Messages
All text configuration is centrally managed inside `index.html`:
```javascript
// Locate the configuration block in index.html
const mockData = {
  titleLetter: 'Happy Birthday!',
  contentLetter: 'To the most wonderful person in my life... 💕',
  signatureLetter: 'With all my love ❤️',
  music: 'happybirthday.mp3'
};
```

### 2. Updating Photos
Replace images in the `image/` directory or update image sources inside `index.html`:
- `photo_cake.jpg` & `photo_roses.jpg` for Polaroid memories.
- `flower.jpg` & `image.jpg` for additional memory deck slides.

### 3. Customizing Scratch Cards
Modify the scratch vouchers under the `renderScratchStage()` method in `index.html` to customize prize titles, rewards, and descriptions.

---

## 📱 Mobile & Performance Optimization

- **Zero Heavy Framework Overhead**: Built with pure Vanilla JS and CSS3 for lightning-fast loads.
- **Hardware Acceleration**: `transform` and `opacity` properties utilized for 60 FPS transitions.
- **Touch Gesture Locks**: Mobile gesture zoom and double-tap zoom prevented for a native app-like experience.
- **Responsive Breakpoints**: Tailored media queries for Desktop (1440px+), Tablet (768px-1024px), and Mobile (<600px).

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.
