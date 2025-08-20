# Electricity Demand Prediction Platform

A full-stack web application for real-time electricity demand prediction, built for the Government of Delhi as part of the Smart India Hackathon 2024.

## 🚀 Project Objective

To provide accurate, real-time, and category-wise (total, commercial, domestic) electricity demand predictions for Delhi using advanced machine learning models, with a modern dashboard for visualization and analytics.

## 🏗️ Tech Stack

**Frontend:**
- Next.js (React 18)
- TypeScript
- Tailwind CSS
- ApexCharts, ECharts, Recharts (Data Visualization)
- Leaflet, React-Leaflet (Mapping)
- Framer Motion (Animations)
- Flowbite, Radix UI (UI Components)
- React Hook Form, Zod (Forms & Validation)
- NextAuth.js (Authentication)

**Backend:**
- Node.js (API routes via Next.js)
- Prisma ORM
- MongoDB (Database)

**Python ML Service:**
- Flask (REST API)
- scikit-learn (Machine Learning)
- pandas, numpy (Data Processing)
- joblib (Model Serialization)
- flask-cors (CORS support)

## 🧠 Machine Learning Models

- **Total Demand Model:** Predicts overall electricity demand using weather, time, and event features.
- **Commercial Demand Model:** Specialized for commercial sector demand.
- **Domestic Demand Model:** Specialized for domestic sector demand.

All models use feature scaling (MinMaxScaler) and are trained with scikit-learn. Models are served via a Flask API and integrated with the Next.js frontend.

## 📁 Project Structure

- `/src` — Next.js frontend (pages, components, API routes, middleware)
- `/python_model` — Python Flask server, ML models, and requirements
- `/prisma` — Prisma schema for MongoDB
- `/public` — Static assets and images

## ⚙️ Key Features

- Real-time demand prediction (total, commercial, domestic)
- Interactive dashboard with charts and maps
- User authentication and role-based access (Admin, Supervisor, Area Manager, User)
- Data stored in MongoDB, managed via Prisma ORM
- Modern, responsive UI with Tailwind CSS

## 📝 How It Works

1. **User logs in** to the dashboard.
2. **Frontend** collects input features (weather, time, etc.) and sends them to the Flask API.
3. **Flask API** preprocesses input, applies the appropriate ML model, and returns predictions.
4. **Frontend** visualizes predictions and analytics in real time.

## 📦 Installation

1. Clone the repo and install Node.js and Python dependencies:
   ```bash
   npm install
   cd python_model
   pip install -r requirements.txt
   ```
2. Set up MongoDB and Prisma.
3. Start the Flask server:
   ```bash
   python server.py
   ```
4. Start the Next.js app:
   ```bash
   npm run dev
   ```

## 🤝 Contributors

- SWETANK SINHA and Team

---
