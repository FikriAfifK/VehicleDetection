# 🚗 VehicleDetection
**Real-Time Vehicle Detection and Traffic Dashboard**

---

## 📌 Overview
This project is a **full-stack vehicle detection and tracking system**.  
It uses a YOLO-based deep learning model for detection and tracking (backend), and a React.js dashboard (frontend) for visualization.  

The system provides:  
- Vehicle detection & tracking from video streams  
- Data visualization (speed, direction, line charts, bar charts)  
- Dashboard with traffic monitoring features  

---

## 📂 Project Structure

### 🔙 Backend (`/backend`)
backend/
│── models/
│ └── best.pt # Trained YOLO model weights
│
│── utils/
│ ├── config.py # Configuration settings
│ ├── detection.py # Vehicle detection logic
│ ├── display.py # Display & visualization utilities
│ ├── save_to_csv.py # Export detection results to CSV
│ ├── tracking.py # Object tracking logic
│ └── view_transformer.py # Perspective/view transformations
│
│── app.py # Backend app (Flask/FastAPI API)
│── main.py # Entry point for backend

### 🎨 Frontend (`/frontend`)
frontend/
│── public/
│ ├── index.html
│ ├── favicon.ico
│ ├── logo192.png, logo512.png
│ └── manifest.json
│
│── src/
│ ├── assets/
│ │ └── Logo_Stempel_HD.png
│ ├── components/
│ │ ├── SimpangAmongrogoDas.js
│ │ ├── SimpangDemanganDas.js
│ │ ├── VehicleDetail.js
│ │ ├── VehicleDirectionBarChart.js
│ │ ├── VehicleLineChart.js
│ │ ├── VehicleSpeedBarChart.js
│ │ ├── VehicleTableChart.js
│ │ └── VideoPlay.js
│ ├── App.js
│ ├── App.css
│ ├── index.js
│ └── ...
│
│── package.json # Frontend dependencies

---

## 🛠️ Technologies & Tools
- **Backend**
  - Python 3.x
  - YOLOv10
  - OpenCV
  - Flask
  - Pandas, NumPy

- **Frontend**
  - React.js
  - Recharts (for charts)
  - CSS

---

## ▶️ How to Run

### 🔙 Backend
1. Go to backend folder:
   ```bash
   cd backend
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
3. Run backend:
   ```bash
   python app.py

### 🎨 Frontend
1. Go to frontend folder:
   ```bash
   cd frontend
2. Install dependencies:
   ```bash
   npm install
3. Start development server:
   ```bash
   npm start
