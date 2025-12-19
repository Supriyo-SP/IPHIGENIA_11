# 🎉 IPHIGENIA 11.0 - IIE Kalyani Fest Website

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Responsive](https://img.shields.io/badge/Responsive-Yes-brightgreen?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)]()

**The Official Website for IPHIGENIA 11.0 - The 11th Anniversary Fest of IIE Kalyani**

[View Demo](#) · [Report Bug](#) · [Request Feature](#)

</div>

---

## 📋 Table of Contents

- [About The Project](#about-the-project)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Customization Guide](#customization-guide)
- [Screenshots](#screenshots)
- [Browser Support](#browser-support)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## 🎯 About The Project

IPHIGENIA 11.0 is the premier 2-day student festival of Indian Institute of Engineering Science and Technology (IIE), Kalyani. This website serves as the digital gateway to the fest, showcasing events, gallery, and registration portals.

### Why This Project?

- 🎨 **Modern Design**: Sleek, dark-themed UI with accent colors that pop
- 📱 **Fully Responsive**: Perfect experience across all devices
- ⚡ **Performance Optimized**: Fast loading with smooth animations
- 🎬 **Custom Video Player**: Themed video player with full controls
- 🎭 **Event Showcase**: Beautiful carousel and event cards

---

## ✨ Features

### 🎪 Core Features

- **Hero Section with Image Carousel** - Auto-rotating showcase images
- **Event Lineup** - Horizontal scrolling cards (mobile) / Grid layout (desktop)
- **Photo Gallery** - Infinite marquee animation with hover effects
- **Custom Video Player** 
  - Custom play button with theme colors
  - Progress bar with seek functionality
  - Volume control with slider
  - Fullscreen support
  - Time display
  - Video poster/banner
- **Smooth Scroll Navigation** - Seamless section transitions
- **AOS Animations** - Scroll-triggered animations
- **Mobile Optimized** - Touch-friendly interface

### 🎨 Design Features

- Dark theme with orange accent (#ff5722)
- Custom scrollbar styling
- Button shine animations
- Floating animations
- Grayscale to color transitions
- Responsive typography
- Hidden scrollbars on mobile (while maintaining functionality)

---

## 🛠️ Tech Stack

### Frontend
- **HTML5** - Semantic markup
- **CSS3** - Custom animations & transitions
- **JavaScript (Vanilla)** - Custom video player & carousel
- **Tailwind CSS** - Utility-first styling via CDN

### Libraries & Frameworks
- **AOS (Animate On Scroll)** - v2.3.1
- **Google Fonts** - Plus Jakarta Sans
- **Tailwind CSS** - v3.x (CDN)

### Assets
- Unsplash API for placeholder images
- Custom video assets

---

## 🚀 Getting Started

### Prerequisites

No build tools or dependencies required! This is a static website that runs directly in the browser.

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/iphigenia-11.git
   cd iphigenia-11
   ```

2. **Add your video file**
   - Create an `assets` folder in the root directory
   - Place your video file in the assets folder
   - Update the video source path in `index.html` (line ~268)

3. **Open in browser**
   ```bash
   # Simply open index.html in your browser
   # Or use a local server (recommended)
   
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (http-server)
   npx http-server
   
   # Using PHP
   php -S localhost:8000
   ```

4. **View the website**
   - Open `http://localhost:8000` in your browser

---

## 📁 Project Structure

```
IPHIGENIA_11/
│
├── index.html          # Main HTML file
├── README.md           # Project documentation
│
└── assets/             # (Create this folder)
    └── video.mp4       # Your fest video
```

---

## 🎨 Customization Guide

### 1. **Update Event Registration Links**

Find the event cards section and replace `href="#"` with your Google Form URLs:

```html
<!-- Line ~222, 231, 240 -->
<a href="YOUR_GOOGLE_FORM_URL" class="...">Register for Tech</a>
```

### 2. **Add Carousel Images**

In the hero section, add more slides:

```html
<!-- Line ~119 -->
<div class="carousel-slide"><img src="IMAGE_URL" alt="Fest Image 2"></div>
<div class="carousel-slide"><img src="IMAGE_URL" alt="Fest Image 3"></div>
```

### 3. **Update Gallery Images**

Replace Unsplash URLs with your own fest photos:

```html
<!-- Line ~252 onwards -->
<img src="YOUR_IMAGE_URL" class="...">
```

### 4. **Change Theme Colors**

Update the accent color in the Tailwind config:

```javascript
// Line ~16
colors: {
    accent: '#ff5722',  // Change this to your color
}
```

### 5. **Update Video**

Replace the video source path:

```html
<!-- Line ~268 -->
<source src="path/to/your/video.mp4" type="video/mp4">
```

### 6. **Update Video Poster**

Change the video thumbnail/banner:

```html
<!-- Line ~267 -->
<video ... poster="YOUR_POSTER_IMAGE_URL">
```

### 7. **Update Contact Information**

Edit footer section:

```html
<!-- Line ~298 -->
<a href="mailto:your-email@example.com" class="text-accent block">Email Us</a>
```

### 8. **Social Media Links**

Update social media buttons:

```html
<!-- Line ~307 -->
<a href="YOUR_FACEBOOK_URL" class="...">FB</a>
<a href="YOUR_INSTAGRAM_URL" class="...">IG</a>
```

---

## 📸 Screenshots

### Desktop View
- Hero section with carousel
- Event lineup cards
- Gallery marquee
- Custom video player

### Mobile View
- Responsive navigation
- Horizontal scrolling events
- Optimized buttons
- Touch-friendly controls

---

## 🌐 Browser Support

| Browser | Version |
|---------|---------|
| Chrome  | ✅ Latest |
| Firefox | ✅ Latest |
| Safari  | ✅ Latest |
| Edge    | ✅ Latest |
| Opera   | ✅ Latest |

**Note**: Custom video controls may vary slightly across browsers due to native video API differences.

---

## 🎬 Video Player Features

The custom video player includes:

- ▶️ **Play/Pause** - Center button + control bar
- 📊 **Progress Bar** - Click to seek
- 🔊 **Volume Control** - Mute/unmute + slider
- ⏱️ **Time Display** - Current / Total duration
- 🖥️ **Fullscreen** - Toggle fullscreen mode
- 🎨 **Themed Design** - Matches site colors
- 📱 **Mobile Optimized** - Touch-friendly controls

---

## 📱 Responsive Design

### Breakpoints

- **Mobile**: < 640px
- **Tablet**: 640px - 1024px
- **Desktop**: > 1024px

### Mobile Optimizations

- Reduced padding and margins
- Horizontal scroll for event cards (no scrollbar)
- Smaller buttons and text
- Optimized navigation bar
- Touch-friendly video controls

---

## 🤝 Contributing

Contributions are what make the open-source community amazing! Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 To-Do List

- [ ] Add more carousel images
- [ ] Integrate backend for form submissions
- [ ] Add event schedule section
- [ ] Create sponsor showcase section
- [ ] Add past year highlights
- [ ] Implement dark/light mode toggle
- [ ] Add loading animations
- [ ] Create admin panel for updates

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 📧 Contact

**IIE Kalyani Student Fest Committee**

- Email: [iiestudentfestcommittee@gmail.com](mailto:iiestudentfestcommittee@gmail.com)
- Location: Kalyani, Nadia, West Bengal

**Project Link**: [https://github.com/yourusername/iphigenia-11](https://github.com/yourusername/iphigenia-11)

---

## 🙏 Acknowledgments

- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- [AOS](https://michalsnik.github.io/aos/) - Animate On Scroll Library
- [Google Fonts](https://fonts.google.com/) - Plus Jakarta Sans
- [Unsplash](https://unsplash.com/) - Free high-quality images
- [Shields.io](https://shields.io/) - README badges

---

<div align="center">

### ⭐ Star this repo if you find it helpful!

Made with ❤️ by IIE Kalyani Students

**© 2025 IPHIGENIA IIE Kalyani | 11th Anniversary Edition**

</div>
