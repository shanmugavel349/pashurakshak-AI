# 🐾 PashuRakshak AI — AI-Powered Livestock Disease Surveillance & Veterinary Response System
> **Smart India Hackathon (SIH 2026)** • Department of Animal Husbandry & Dairying (DAHD) • Ministry of Fisheries, Animal Husbandry & Dairying

---

## 📌 Executive Summary & National Impact
Livestock farming contributes over **5% of India's national GDP** and sustains **80+ Million rural livelihoods**. However, contagious viral & bacterial epizootics—such as **Foot-and-Mouth Disease (FMD)**, **Lumpy Skin Disease (LSD)**, **Haemorrhagic Septicaemia (HS)**, and **Anthrax**—inflict annual economic losses exceeding **₹30,000+ Crore** due to:
1. **Reporting Delays (5–8 days):** Traditional physical dispensary visits allow high-$R_0$ viruses to spread rapidly across village herds.
2. **Language & Literacy Barriers:** Complex text-based portals alienate rural farmers who communicate primarily in regional vernacular dialects.
3. **Lack of Early Spatial Containment:** Absence of automated geospatial containment zone calculations (3km red rings & 10km buffer zones) delays ring vaccination.

**PashuRakshak AI** solves this through a unified, voice-first intelligent surveillance ecosystem connecting **Farmers**, **Block Veterinary Surgeons**, and **State Epidemiological Command Centers** in real time.

---

## 🌟 Key Features & Workflow Architecture

```
[ Rural Farmer ]
     │
     ├─► Multilingual AI Voice Call (Tamil / Hindi / Telugu / English / Kannada)
     ├─► Smart App Form with AI Vision Lesion Detection (Bounding Box Overlay)
     │
     ▼
[ AI Clinical Triage Engine ]
     │
     ├─► NLP Entity Extraction (Species, Symptoms, Duration, Severity)
     ├─► Differential Pathogen Classifier (10 Critical Diseases)
     ├─► Contagion Index (R₀) & Risk Level Calculation (Critical, High, Medium, Low)
     ├─► Instant Localized First-Aid & Biosecurity Advice
     │
     ▼
[ Veterinary Tele-Triage Desk ]
     │
     ├─► Priority Incoming Emergency Queue & Case Files
     ├─► 1-Click Mobile Clinic / Field Visit Dispatch
     ├─► Diagnostic Lab Sample Orders (RT-PCR, ELISA, California Mastitis Test)
     ├─► Signed Digital Prescription (Rx) with Mandatory Quarantine Days
     │
     ▼
[ State Epidemiological Command Center ]
     │
     ├─► GIS Spatial Heatmaps with Automated 3km Red Containment & 10km Buffer Zones
     ├─► 7-Day Outbreak Incidence & Ring Vaccination Coverage Curves
     ├─► Multi-Channel Mass Public Alert Broadcast (SMS, App Push, Voice IVR)
     ├─► Vaccine Cold-Chain Logistics & District Inventory Tracker (2°C - 8°C)
```

---

## 💻 Tech Stack

| Layer | Technologies |
|---|---|
| **Frontend Framework** | React 19, Vite, TypeScript |
| **Backend API** | Python FastAPI, Uvicorn, SQLite, SQLAlchemy ORM, Pydantic v2 |
| **Styling & UI** | Tailwind CSS 3.4, Lucide Icons, Custom Equalizers |
| **GIS Mapping** | Leaflet, React-Leaflet (Geodesic circular containment overlays) |
| **Data Visualization** | Chart.js, React-Chartjs-2 (Multi-axis epidemiological curves) |
| **Speech & Voice AI** | Web Speech Recognition API + Multilingual NLP Entity Extraction (`ta-IN`, `hi-IN`, `te-IN`, `en-IN`, `kn-IN`) |
| **Clinical Diagnostic Engine** | Differential Pathogen Risk Matrix (10 Critical Epizootics), Bounding Box Lesion Detection, Contagion Index ($R_0$) |
| **State & Data Synchronization** | React Context + Live REST API Client + SQLite Auto-Seeding Persistence |

---

## 🚀 Getting Started & Run Commands

### 1. Start the Backend API (FastAPI + SQLite)
In one terminal tab:
```bash
cd ~/projects/pashurakshak-ai/backend
./run.sh
```
* **API Server:** `http://localhost:8000`
* **Interactive Swagger API Docs:** `http://localhost:8000/docs`
* **Health Check:** `http://localhost:8000/api/health`

### 2. Start the Frontend Development Server (React + Vite)
In a second terminal tab:
```bash
cd ~/projects/pashurakshak-ai
npm run dev
```
* **Frontend App:** `http://localhost:5173`

### 3. Build Frontend for Production
```bash
cd ~/projects/pashurakshak-ai
npm run build
```


---

## ⚡ 1-Click Live SIH Demo Pitch Guide

When presenting to hackathon judges:
1. **Top Navigation Bar:** Click the red **`⚡ Simulate Outbreak`** button or switch to the **`🏆 SIH Pitch`** tab.
2. Select **`🚨 FMD Index Outbreak (Tamil)`**.
3. Watch the system execute the full **6-stage lifecycle** live in under 30 seconds:
   - **Step 1:** Voice input auto-extracts species (`Jersey Cow`), symptoms (`Mouth Blisters`, `Drooling`, `Lameness`), and duration (`2 days`).
   - **Step 2:** AI Triage flags **Foot-and-Mouth Disease (95.8% Confidence, CRITICAL, R₀: 4.8)**.
   - **Step 3:** Veterinarian receives emergency notification with GPS map pin and schedules field visit.
   - **Step 4:** RT-PCR lab sample is dispatched with live positive result return.
   - **Step 5:** Doctor signs official digital prescription (Rx) with mandatory 14-day quarantine.
   - **Step 6:** State HQ activates **3km Red Containment Zone** and triggers emergency mass SMS/Voice broadcast to 16,840 farmers.

---

## 👥 Authors & Team
- **Shanmugavel R** (Reg No: `2503737716921033`)
- **Institution:** K.S. Rangasamy College of Technology
- **Hackathon:** Smart India Hackathon (SIH 2026)
