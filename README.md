# Sonic Sketchpad 🎨🎵

An interactive audio-visual drawing application. Draw with your mouse or touch to create art and music simultaneously!

## Palm Lotus 🪷

`palm-lotus.html` is a separate app: a 3D lotus that opens when you open your hand and closes when you make a fist. It uses your webcam and Google's MediaPipe hand tracker, which runs inside the browser, so no video leaves your computer.

To use it, open `palm-lotus.html` in Chrome or Edge (double-clicking the file works), click **Start camera** and allow camera access. It needs an internet connection the first time it loads. If you don't have a camera, **Use a slider instead** opens and closes the lotus by hand.

## Features
- Real-time audio synthesis based on drawing position
- Multiple waveforms (Sine, Square, Sawtooth)
- Color palette for artistic expression
- Delay/echo effects
- Ambient drone backing track
- Save your artwork as PNG

## 🚀 Quick Start

### Local Deployment

**Option 1: Python Server (Simplest)**
```bash
# Python 3
python3 -m http.server 8000

# Then open: http://localhost:8000
```

**Option 2: Node.js Server**
```bash
# Install a simple server globally
npm install -g http-server

# Run it
http-server -p 8000

# Then open: http://localhost:8000
```

**Option 3: PHP Server**
```bash
php -S localhost:8000
```

### 🌐 Online Deployment

#### Deploy to GitHub Pages (Free)
1. Push this repository to GitHub
2. Go to repository Settings → Pages
3. Select branch to deploy from
4. Your site will be live at: `https://yourusername.github.io/sonicdraw/`

#### Deploy to Netlify (Free, Easiest)
1. Visit [netlify.com](https://netlify.com)
2. Drag and drop this folder, or connect your Git repository
3. Done! Instant deployment with HTTPS

#### Deploy to Vercel (Free)
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

#### Deploy to Cloudflare Pages (Free)
1. Visit [pages.cloudflare.com](https://pages.cloudflare.com)
2. Connect your Git repository
3. Deploy automatically

## Usage

1. Click "Start Experience" to initialize audio
2. Draw on the canvas with your mouse or finger
3. X-axis controls pitch, Y-axis controls filter frequency
4. Switch instruments, colors, and adjust delay
5. Save your artwork when done!

## Technical Details
- Pure HTML/CSS/JavaScript - no build process required
- Web Audio API for sound synthesis
- Canvas 2D for drawing
- Tailwind CSS (via CDN) for styling
- Works on desktop and mobile devices

## Browser Requirements
- Modern browser with Web Audio API support
- Chrome, Firefox, Safari, Edge (latest versions)
- User gesture required to start audio (browser security)
