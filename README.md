# Ashmit Singh | VLSI & Robotics Engineer Portfolio

A static portfolio website showcasing Ashmit Singh's work in VLSI design and robotics engineering. Built with a custom dc-runtime framework and features smooth 3D transitions between pages.

## Overview

This portfolio website presents two main sections:

### VLSI Side
- VLSI project showcases (Harris Corner Detector ASIC, Load-Aware Adaptive H-Bridge, Reliability-Aware DFT, PID Hardware Accelerator)
- VLSI resume download
- Electronics engineering background

### Robotics Side
- Robotics project showcases (Warehouse DWS, Team Vyadh Robotic Arm, Gesture-Controlled Arm)
- Robotics resume download
- Soft robotics & actuator research focus

## Features

- **Smooth 3D page transitions** - Circular cube flip and carousel-style rotations between sections
- **Responsive design** - Works on both desktop (1440px) and mobile (390px) with separate home-m.html
- **Interactive elements** - Animated gradients, hover effects, and scroll-in animations
- **SEO optimized** - Meta tags, Open Graph tags, Twitter cards, and JSON-LD structured data
- **Performance focused** - Static site with no build step, pre-configured Vercel caching
- **Dark theme** - Consistent #07070C dark background across all pages

## Page Structure

| Page | Description |
|------|-------------|
| `index.html` | Main shell with routing between sections (#home, #vlsi, #robotics, #about, #projects) |
| `pages/home.html` | Desktop landing page with scrolling text intro and VLSI/Robotics CTA buttons |
| `pages/home-m.html` | Mobile-optimized landing page (390px width) |
| `pages/vlsi.html` | VLSI section with project grid |
| `pages/robotics.html` | Robotics section with project grid |
| `pages/about.html` | About page with contact info and social links |
| `pages/projects.html` | Projects carousel with filterable chips by category |

## Technical Details

- **Framework**: Custom dc-runtime framework with DCLogic base class
- **Rendering**: React used for component mounting (`react.production.min.js`, `react-dom.production.min.js`)
- **Assets**: Manrope font, custom SVG icons, project images
- **Deployment**: Vercel with `framework: null`, `outputDirectory: "."`
- **Fonts**: Manrope (weights 200-800) with latin and latin-ext unicode ranges

## Projects Showcased

### VLSI Projects
1. **Harris Corner Detector ASIC** - SystemVerilog streaming detector with Genus/Innovus routing and Conformal LEC verification
2. **Load-Aware Adaptive H-Bridge** - Brushed-DC motor driver sensed at 90nm in Cadence with adaptive PWM
3. **Reliability-Aware DFT** - Robotic SoC with MBIST and reliability-aware scheduler (Python, Yosys)
4. **PID Hardware Accelerator** - RTL PID controller at the intersection of robotics, control, and VLSI

### Robotics Projects
1. **Warehouse DWS at Delhivery** - Parcel-measuring station with Intel RealSense D455, point-cloud vision (RANSAC, PCA), ROS2, FastAPI
2. **Team Vyadh Robotic Arm** - Mars rover arm control: ROS 2 Jazzy on Jetson, STM32 motor control, AS5600 encoders
3. **Gesture-Controlled Arm** - OpenCV/MediaPipe hand tracking → WiFi → ESP32 → joint control, Arduino integration

## Deployment

This is a static site deployable to Vercel:

1. Push this repository to GitHub
2. Create a new Vercel project, linking to this repo
3. Framework Preset: "Other" (vercel.json already sets this)
4. Run `vercel --prod` or deploy via dashboard

## Directory Contents

- `index.html` - Shell, transitions, routing, SEO and share-card tags
- `pages/` - Home, home-m (mobile), VLSI, Robotics, About, Projects
- `assets/` - Fonts, React runtime, images, favicon
- `resume-vlsi.pdf`, `resume-robotics.pdf` - Downloadable resumes
- `og-card-v2.png` - Share card image
- `vercel.json` - Vercel configuration (null framework, caching headers)
- `DEPLOY.md` - Detailed deployment instructions

## License

Personal portfolio - all rights reserved.