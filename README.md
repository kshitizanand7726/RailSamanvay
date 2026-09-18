# RailSamanvay (रेल समन्वय) 🚆🇮🇳
### AI-Powered Automatic Block Planning & Multi-Department Corridor Coordination
**Smart India Hackathon (SIH) Problem Statement: SIH26027**  
*Organization:* Ministry of Railways, Government of India  
*Corridor:* Ghaziabad – Kanpur (NCR High-Density Network)

---

## 📌 Problem Overview
Maintenance blocks across Indian Railways traditionally require manual coordination across disparate departments (Civil/TMS, Electrical/TDMS, Signal/SMMS). When unexpected defects or traffic variations occur, piecemeal block granting leads to severe congestion, train delays, and sub-optimal track availability.

**RailSamanvay** introduces an AI-powered multi-department shadow scheduling engine using Constraint Satisfaction Optimization (CP-SAT) to:
- Automatically identify shadow maintenance windows between high-speed train movements.
- Bundle cross-departmental demands (Civil, Electrical, Signal) into unified, conflict-free windows.
- Intelligently adapt to real-time delay perturbations and emergency weld fracture alerts without disrupting critical passenger corridors.

---

## ⚡ Key Features
- **Constraint Programming Optimization**: Mathematical guarantee of safety buffers and zero-conflict paths.
- **Dynamic Multi-Department Bundling**: Combines track tamping, OHE overhaul, and point machine maintenance to maximize asset utilization.
- **Live Interactive GIS Map**: Visualizes multiple track lines (Up Main, Down Main, Siding) with Standard, Satellite (with place labels), and Terrain layers.
- **Interactive Marey Chart (Time-Distance Graph)**: Staggered, collision-free train trajectories with clear maintenance shadow visualizers.
- **Emergency Defect Injection**: One-click instant rescheduling on critical track alarms (e.g., Rail Weld Fracture).
- **Train Radar & Division ETA Tracker**: Real-time position tracking and division arrival calculations by train name or number.
- **Persistent Historical Archive**: Preserves completed blocks and past train runs for audit and analytics.

---

## 🛠️ Quick Start

### 1. Prerequisites
- Python 3.10+
- Git

### 2. Installation
`ash
# Clone the repository
git clone https://github.com/<YOUR_USERNAME>/RailSamanvay.git
cd RailSamanvay

# Create a virtual environment
python -m venv venv

# Activate virtual environment
# Windows:
.\venv\Scripts\activate
# Linux/macOS:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
`

### 3. Running the Application
`ash
python -m uvicorn main:app --reload --port 8000
`
Open your browser and navigate to:
`	ext
http://127.0.0.1:8000
`
