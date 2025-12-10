# 🎠 Rotating Image Gallery

## Preview

![Rotating Gallery Demo](src/Animation.gif)

*A smooth 3D rotating image gallery with interactive navigation*

---

## 📋 Description

A beautiful, interactive 3D rotating image gallery built with vanilla HTML, CSS, and JavaScript. The gallery displays images in a circular carousel that rotates smoothly with automatic rotation and manual navigation controls.

## ✨ Features

- **3D Perspective Effect**: Images arranged in a 3D circular carousel using CSS transforms
- **Smooth Animations**: Seamless transitions with 0.7s animation duration
- **Auto-Rotation**: Gallery automatically rotates every 3 seconds
- **Manual Controls**: Previous and Next buttons to control rotation manually
- **Responsive Design**: Clean, centered layout that works across devices
- **Hover Effects**: Interactive button styling with brightness effect
- **8 Images**: Displays 8 images in a circular arrangement (45° spacing)

## 🚀 Quick Start

### Installation

1. Clone or download this project
2. Open `index.html` in your web browser
3. That's it! No dependencies required

### Usage

- Click **Prev** button to rotate gallery counter-clockwise
- Click **Next** button to rotate gallery clockwise
- Gallery auto-rotates every 3 seconds when idle
- Clicking buttons resets the auto-rotation timer

## 🛠️ Technical Details

### Technologies Used
- **HTML5**: Semantic markup
- **CSS3**: 3D transforms, perspective, and animations
- **JavaScript (Vanilla)**: Event handling and DOM manipulation

### How It Works

1. **3D Carousel**: Images are positioned in 3D space using CSS `transform: rotateY()` and `translateZ()`
2. **Rotation**: JavaScript updates the container's `rotateY` transform based on user interaction
3. **Auto-play**: `setTimeout` triggers automatic rotation every 3 seconds
4. **Event Handling**: Click events on buttons update the rotation angle (45° per image)

### Project Structure

```
Rotating Image Gallery/
├── index.html      # HTML structure
├── style.css       # Styling and animations
├── index.js        # JavaScript logic
└── Readme.md       # This file
```

## 📝 Files Overview

| File | Purpose |
|------|---------|
| `index.html` | Contains the gallery structure with 8 images and control buttons |
| `style.css` | Handles 3D transforms, animations, and button styling |
| `index.js` | Manages rotation logic, auto-play, and user interactions |

## 🎨 Customization

### Change Number of Images
- Modify the `<span>` elements in `index.html`
- Update the angle calculation: `360 / number_of_images`
- Update `translateZ` value for depth effect

### Change Colors
- Background: Edit `background-color` in `body` selector
- Button color: Edit `background-color` in `.btn` selector

### Adjust Animation Speed
- Rotation duration: Change `0.7s` in `.image-container` transition
- Auto-rotation interval: Change `3000` (milliseconds) in `index.js`

## 📸 Image Sources

Currently using [Picsum Photos](https://picsum.photos/) for demo images. Replace `src` attributes in `index.html` with your own images.

## 💡 Notes

- The gallery displays 8 images arranged in a circle
- Each image rotates 45° from the previous one (360° / 8 = 45°)
- The `--i` CSS variable is used for calculating individual image positions
- `perspective(1000px)` creates the 3D depth effect

## 📄 License

Free to use and modify for personal and commercial projects.

---

**Enjoy your rotating gallery! 🎞️**
