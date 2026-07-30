# Hardware Component Detector

An end-to-end Computer Vision web application designed to detect and classify hardware components in real-time. Powered by a custom-trained model on **5,000 annotated images across 24 hardware classes**, this project integrates serverless edge proxies for low-latency, zero-CORS inference and dynamic browser rendering via HTML5 Canvas.

#### Website link:https://hardware-component-detector.netlify.app/
---

##  Key Features

- **Custom ML Pipeline:** Trained on 5,000 images covering 24 distinct hardware categories via Roboflow Workflows.
- **Dynamic Bounding Box Overlay:** Uses HTML5 Canvas API to calculate and render precise bounding boxes and confidence percentages over input images.
- **Zero-CORS Edge Routing:** Implements serverless edge proxies (Cloudflare Workers / Netlify Redirects) to safely route API calls without cross-origin issues.
- **Responsive & Modern UI:** Glassmorphism UI styling with support for Dark and Light themes.
- **Audio Feedback:** Utilizes the Web Audio API for custom audio chimes upon successful detection.
- **Flexible Image Inputs:** Supports both live camera capture and gallery file uploads.

---

##  Tech Stack

### **Frontend**
- **HTML5 & CSS3:** Flexbox/Grid layouts, Glassmorphism, CSS Variables for Dark/Light themes.
- **Vanilla JavaScript (ES6+):** Async/Await, Fetch API, FileReader API.
- **HTML5 Canvas API:** Real-time object bounding box calculation and rendering.
- **Web Audio API:** Synthetic sound generation on detection.

### **Machine Learning & Data Processing**
- **Dataset:** 5,000 image samples across 24 hardware classes.
- **Annotation & Workflow Engine:** Roboflow Workflows (`finalmldataset-v2-logic`).

### **Backend & Deployment**
- **Proxy Layer:** Cloudflare Workers / Netlify Redirects (`_redirects` / `netlify.toml`).
- **Hosting:** Netlify / Cloudflare Pages.

---

##  Dataset & Model Overview

| Metric | Details |
|---|---|
| **Total Images** | 5,000 |
| **Classes** | 24 Hardware Categories |
| **Annotation Tool** | Roboflow |
| **Inference Engine** | Roboflow Serverless Workflows API |

---

##  Project Structure

```text
├── index.html         # Main Application UI & Logic
├── _redirects         # Proxy redirect config for Netlify / Cloudflare Pages
├── netlify.toml       # Netlify serverless routing configuration (optional)
├── tanvir.jpg         # Profile image
└── README.md          # Project documentation
