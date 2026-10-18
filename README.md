# phytospore-edge

# 🌾 PhytoSpore Edge
> **Pre-Symptomatic Crop Defense via Offline Edge-AI & Optical Macro-Diagnostics**  
> *Technovation Girls 2026–2027 Senior Division Submission*

---

## 📌 Executive Overview
Fungal plant pathogens destroy over **40% of global staple crop yields** annually. Traditional crop diagnostic mobile apps rely on **post-symptomatic detection**—analyzing visual damage after leaf lesions or yellowing appear. By then, host plant cells are compromised, forcing farmers to apply costly and toxic chemicals.

**PhytoSpore Edge** shifts crop defense to **pre-symptomatic prevention**. By combining a $5 clip-on smartphone optical macro lens with adhesive air-sampling tape, smallholder farmers capture microscopic images of airborne spores *before* infection sets in. 

Running a quantized **YOLOv8s-SPM** model via TensorFlow Lite, the app executes 100% offline in **<300 milliseconds**, calculating a **Spore Density Index (SDI)** to recommend early, organic bio-fungicide treatments.

---

## 🛠️ Key Features & System Architecture

- **Offline Edge ML:** Quantized INT8 TensorFlow Lite model (<8MB binary footprint) running locally on budget mobile hardware.
- **Optical Preprocessing:** Automated CameraX pipeline featuring **Laplacian variance sharpness filtering** ($\sigma^2 > 70$) and **CLAHE contrast enhancement**.
- **Privacy-First Data Storage:** Encrypted local **SQLite** log storage ensuring zero cloud dependency or land data tracking.
- **Global Multi-Language UI:** Native localization supporting **English**, **Hindi (हिन्दी)**, and **Spanish (Español)**.
- **Role-Based Portals:** Dedicated access modes for **Smallholder Farmers** (scanning & action plans) and **Cooperative Managers** (regional outbreak heatmaps).

---

## 🚀 Quickstart & Local Setup

### 1. Prerequisites
Ensure you have Python 3.10+ installed on your system.

### 2. Installation
Clone this repository and install the required dependencies:
```bash
git clone [https://github.com/your-username/phytospore-edge.git](https://github.com/your-username/phytospore-edge.git)
cd phytospore-edge
pip install -r requirements.txt
