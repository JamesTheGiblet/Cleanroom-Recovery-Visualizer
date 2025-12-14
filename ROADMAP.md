# Product Roadmap: Cleanroom Intelligence Platform

This roadmap outlines the strategic development phases from the current MVP (Prototype) to a fully integrated IoT Enterprise Solution.

## 🚩 Phase 1: The Simulator (Current Status)

**Goal:** Field-ready tool for training and scenario planning.

* [x] **Core Logic Engine:** Implementation of exponential decay algorithms.
* [x] **Interactive UI:** Mobile-responsive dashboard with slider controls.
* [x] **Scenario Builder:** Preset events (Spills, Door Open, Equipment Move).
* [x] **Visual Feedback:** Real-time graphing of recovery curves vs. ISO limits.
* [x] **Zero-Install Deployment:** Single-file HTML architecture.
* [x] **State Persistence:** Configuration and event history saved to LocalStorage.
* [x] **Mobile Optimization:** Touch gestures and iOS-specific enhancements.

---

## 🚧 Phase 2: The Integration (Q2 2026)

**Goal:** Connect the visualizer to real-world facility data.

* [ ] **Pro Reporting Suite:** Unlock PDF generation and CSV data export (Currently in Demo Mode).
* [ ] **Cost Analysis Module:** Unlock energy consumption and HVAC cost estimation.
* [ ] **API Connector:** Ability to fetch live `ACH` values from Building Management Systems (BMS).
* [ ] **Multi-Room Support:** Dashboard view for monitoring multiple zones simultaneously.

---

## 🔭 Phase 3: The Enterprise Twin (Q4 2026)

**Goal:** Real-time Digital Twin connected to Lighthouse Particle Counters.

* [ ] **IoT Integration:** Direct ingestion of live particle data via MQTT/WebSocket from LWS Apex sensors.
* [ ] **Predictive Alerting:** AI model to predict "Time to Contamination" before it happens based on trends.
* [ ] **3D Visualization:** WebGL representation of airflow patterns and dead zones.

---

## 💡 Future Concepts

* **AR Overlay:** Using tablet cameras to visualize contamination clouds in AR for training.
* **Compliance Bot:** Automated Slack/Teams notifications when recovery times exceed SOP limits.
