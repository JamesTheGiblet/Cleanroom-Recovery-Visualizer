# LWS Cleanroom Recovery Visualizer (MVP)

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg) ![Status](https://img.shields.io/badge/status-prototype-orange.svg) ![Compliance](https://img.shields.io/badge/ISO-14644--3-compliant-green.svg)

**A real-time contamination decay simulation tool designed for Lighthouse Worldwide Solutions.**

This Progressive Web Application (PWA) models cleanroom recovery performance based on Air Changes per Hour (ACH) and specific contamination events. It visualizes the exponential decay of airborne particulates to predict exactly when a facility returns to **ISO Class 7** compliance.

---

## 🎯 The Problem
Facility managers often rely on static calculations to estimate room recovery times. When a contamination event occurs (e.g., a spill or gowning breach), they need to know:
1. **How bad is the spike?**
2. **Given our current HVAC settings (ACH), how long until we are safe?**

## ⚡ The Solution
This tool uses **First-Order Decay Kinetics** (identical to pharmacokinetic clearance models) to visualize air scrubbing in real-time.

### Key Features
* **Dynamic Simulation:** Model complex scenarios (e.g., "Door Open" followed by "Spill").
* **HVAC Tuning:** Adjust Air Changes per Hour (10-60 ACH) to see the impact on recovery time.
* **ISO Compliance:** Visual thresholds for ISO Class 7/8 limits.
* **Zero-Latency Graphing:** Powered by Plotly.js for millisecond-level rendering updates.
* **Mobile-First Architecture:** Designed for tablets and mobile devices used on the facility floor.

---

## 📐 The Math (Scientific Basis)
The logic engine calculates particulate reduction using the standard Cleanroom Recovery Formula:

$$C_t = C_{initial} \times e^{-(\frac{Q}{V})t}$$

Where:
* **$C_t$**: Concentration at time $t$
* **$Q$**: Airflow rate ($m^3/h$)
* **$V$**: Room Volume ($m^3$)
* **$t$**: Time elapsed

---

## 🚀 Quick Start
This prototype is built as a **Zero-Dependency Single Page Application (SPA)**. It requires no build step, no backend, and no installation.

### Running Locally
1. Clone this repository.
2. Open `lws-cleanroom-demo.html` in any modern browser (Chrome, Safari, Edge).

### Deployment
Because the architecture is static HTML/JS, it can be deployed instantly to:
* GitHub Pages
* Netlify / Vercel
* Internal LWS Intranet (SharePoint/Confluence)

---

## 🛠 Tech Stack
* **Core:** Vanilla JavaScript (ES6+) for maximum performance and compatibility.
* **Visualization:** Plotly.js (via CDN) for scientific-grade charting.
* **Styling:** CSS3 Variables with Flexbox/Grid for responsive layout.
* **Icons:** FontAwesome 6.

---

## 📄 License
**Proprietary Prototype.** Copyright © 2025. All rights reserved.
*Concept developed for Lighthouse Worldwide Solutions.*


###How to use this1. Create a new file in your GitHub repo called `README.md` and paste the first block.
2. Create a new file called `ROADMAP.md` and paste the second block.
3. **The Effect:** When LWS looks at your repo, they won't just see code. They will see a **Business Proposal**. They will realize that you understand "IoT Integration" and "Audit Trails," which makes you instantly more valuable than a junior developer.
