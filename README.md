# 🎬 CODE INJECTOR 2 VIDEO (Universal Code Renderer)

**Live Demo:** [code-injector-to-video.netlify.app](https://code-injector-to-video.netlify.app/)

A browser-based, zero-backend utility designed to seamlessly bridge the gap between generative web art (p5.js, Three.js, vanilla Canvas) and professional video production pipelines. 

This project was built entirely via **AI-assisted Vibe Coding**, demonstrating how LLMs can be utilized to rapidly prototype and deploy custom production tools.

## 💡 Why This Exists?
As a video artist, extracting high-quality, smooth video from web-based generative animations is often a bottleneck. Screen recording software can cause frame drops and compression artifacts. **Code Injector 2 Video** solves this by using the browser's native `MediaRecorder API` to directly capture the `<canvas>` stream and export it into broadcast-ready video files.

## ✨ Key Features
* **Direct Canvas Capture:** Records WebGL/2D Canvas at a stable framerate (25/30/60 FPS) without screen tearing.
* **Broadcast Resolutions:** Presets for 1080p (Horizontal/Vertical for Shorts), Square, and 4K UHD. The iframe scales dynamically without breaking the layout.
* **URL Code Injection:** Built-in proxy fetcher to bypass CORS. You can paste a link to an external web animation, and the tool will parse it, inject a `<base>` tag for assets, and render it.
* **Format Selection:** Export as `MP4` or `WEBM` (Alpha channel support for overlays in After Effects/Premiere).
* **Zero Backend:** The entire recording and rendering process happens client-side in the browser. 

## 🛠 Tech Stack & Methodology
* **Methodology:** AI Vibe Coding (Prompt-driven development)
* **Technologies:** HTML5, CSS3 (Glassmorphism UI), Vanilla JavaScript
* **APIs:** `MediaRecorder API`, `captureStream()`

## 🚀 How to Use
1. Open the tool and click the center **CODE INJECTOR** button to reveal the UI panel.
2. Paste your generative code (HTML/JS) into the editor or fetch it via URL.
3. Select your desired Resolution, Framerate, and Export Format.
4. Click **PREVIEW** to test the animation.
5. Click **EXPORT** (or set an auto-stop duration). The browser will render the frames and automatically download the compiled video file.
