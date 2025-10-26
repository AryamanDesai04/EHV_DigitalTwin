# EHV Digital Twin – AI-Powered Predictive Substation Intelligence Platform  

### Smart India Hackathon 2025 | Team Code Titans | Problem ID: 25191  

---

## 🧠 Overview
**EHV Digital Twin** is a real-time AI-powered simulation and monitoring platform for **400/220 kV substations**, designed to predict faults, detect anomalies, and optimize performance.  
It creates a **virtual mirror** of physical assets — transformers, breakers, CT/CVTs, isolators, reactors, and busbars — enabling predictive diagnostics, live visualization, and operator training.

---

## 🏗️ System Architecture
```mermaid
flowchart TD
A[Physical Substation Assets] --> B[IoT & SCADA Sensors]
B --> C[Data Processing Layer: Pandas, NumPy]
C --> D[Digital Twin Core Engine: ML Models (RF, LSTM)]
D --> E[API & Communication Layer: Flask + WebSocket]
E --> F[Visualization Layer: Plotly Dash Dashboard]
F --> G[Deployment Layer: Docker + Security]
````

Each layer ensures continuous synchronization between physical and digital entities, providing real-time insights and simulation capabilities.

---

## 🧩 Features

* 🔁 **Real-time Virtual Replication** of EHV substation assets
* 🤖 **AI/ML Fault Prediction & Anomaly Detection** (Random Forest, Isolation Forest, LSTM)
* 🧮 **Edge Data Processing** and Local Storage (SQLite, CSV)
* 📡 **IoT/SCADA Integration** via MQTT & OPC-UA
* 🎛️ **Interactive Dashboard** for Voltage, Load, Temperature, and Asset Health
* ⚡ **Fault Simulation Engine** for overload, trip, and short-circuit scenarios
* 🔐 **AES-256 Encrypted Communication** with Role-based Access
* 🐳 **Dockerized Deployment** for cloud or edge environments

---

## 🧰 Tech Stack

| Layer                | Technologies / Frameworks               |
| -------------------- | --------------------------------------- |
| **Programming**      | Python 3.10                             |
| **Machine Learning** | scikit-learn, TensorFlow, NumPy, pandas |
| **Visualization**    | Dash, Plotly, HTML/CSS                  |
| **Backend / APIs**   | Flask, WebSocket, REST API              |
| **Data Layer**       | SQLite, CSV, Pandas                     |
| **Integration**      | MQTT, OPC-UA                            |
| **Deployment**       | Docker, Cloud/Edge Hybrid               |
| **Security**         | AES-256, Token Authentication           |

---

## 🧪 Prototype & Demonstration

Prototype visuals and screenshots are stored in the repository at:
📂 **`/prototype_images/`**

These include:

* Dashboard Interface
* Fault Simulation View
* Asset Health Visualization
* Real-time Parameter Monitoring

---

## ⚙️ Installation & Setup

### Prerequisites

* Python 3.10+
* Docker (optional, for deployment)
* pip

### Steps

```bash
# Clone the repository
git clone https://github.com/<your-username>/EHV-Digital-Twin.git
cd EHV-Digital-Twin

# Install dependencies
pip install -r requirements.txt

# Run Flask API backend
python app.py

# Access dashboard (default: http://127.0.0.1:8050)
```

---

## 📡 Real-Time Data Flow

1. **IoT/SCADA Sensors** → Data streamed via MQTT/OPC-UA
2. **Processing Layer** → Cleaning & feature extraction (pandas, NumPy)
3. **Twin Core** → ML inference for anomaly & fault detection
4. **API Bridge** → JSON data via Flask + WebSocket
5. **Visualization Layer** → Dash dashboard updates in real-time

---

## 🔒 Security & Deployment

* AES-256 encrypted communication channels
* Role-based authentication
* Dockerized microservices for scalable deployment
* Supports both **cloud** and **on-premise** architectures

---

## 📚 Research References

* [CIGRÉ Technical Brochure 815 – Digital Twin for Power Systems](https://e-cigre.org/publication/815-digital-twin-for-power-systems)
* [IEEE Transactions on Power Delivery – AI-Driven Predictive Maintenance (2022)](https://ieeexplore.ieee.org/)
* [CEA Reports on Substation Automation Standards](https://cea.nic.in/)
* [Scikit-learn Documentation](https://scikit-learn.org/stable/)
* [ABB Ability™ Digital Twin Architecture](https://new.abb.com/process-automation/digital/abb-ability-digital-twin)
* [National Grid UK – Digital Substation Roadmap (2023)](https://www.nationalgrid.com/)

---


- The **prototype images** folder mention ensures reviewers can find visuals instantly.  
- All tool names are properly highlighted for visibility during evaluation.  

Would you like me to tailor this README for **public submission polish** (with badges like “Built with Python”, “Docker Ready”, etc.) — or keep it **purely technical for SIH evaluators**?
```
