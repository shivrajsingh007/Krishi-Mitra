# 🌾 KrishiMitra – Smart Farming Assistant

A full-stack web application for Indian farmers with crop management, live market prices, weather forecasts, soil health tracking, expert advisories, and a farming community.

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React 18, React Router v6, Recharts, Lucide Icons |
| Backend | Node.js, Express.js |
| Database | MongoDB (Mongoose ODM) |
| Auth | JWT (JSON Web Tokens) |
| Styling | Pure CSS with CSS Variables |

---

## 📁 Project Structure

```
krishimitra/
├── backend/
│   ├── config/
│   │   └── seed.js          # Database seeder
│   ├── middleware/
│   │   └── auth.js          # JWT middleware
│   ├── models/
│   │   ├── User.js
│   │   ├── Crop.js
│   │   ├── MarketPrice.js
│   │   ├── SoilTest.js
│   │   ├── Advisory.js
│   │   └── Community.js
│   ├── routes/
│   │   ├── auth.js
│   │   ├── crops.js
│   │   ├── weather.js
│   │   ├── market.js
│   │   ├── advisory.js
│   │   ├── soil.js
│   │   ├── community.js
│   │   └── dashboard.js
│   ├── .env
│   ├── package.json
│   └── server.js
└── frontend/
    ├── public/
    │   └── index.html
    ├── src/
    │   ├── components/
    │   │   └── layout/
    │   │       ├── Layout.js
    │   │       └── Layout.css
    │   ├── context/
    │   │   └── AuthContext.js
    │   ├── pages/
    │   │   ├── Landing.js / .css
    │   │   ├── Login.js / Auth.css
    │   │   ├── Register.js
    │   │   ├── Dashboard.js / .css
    │   │   ├── Crops.js / .css
    │   │   ├── Weather.js / .css
    │   │   ├── Market.js / .css
    │   │   ├── Advisory.js / .css
    │   │   ├── Soil.js / .css
    │   │   ├── Community.js / .css
    │   │   └── Profile.js / .css
    │   ├── App.js
    │   ├── index.js
    │   └── index.css
    └── package.json
```

---

## 🚀 How to Run on Your Device

### ✅ Prerequisites – Install These First

1. **Node.js** (v18 or higher)
   - Download from: https://nodejs.org
   - Verify: `node --version`

2. **MongoDB** (Community Edition)
   - Download from: https://www.mongodb.com/try/download/community
   - OR use MongoDB Atlas (free cloud): https://www.mongodb.com/atlas
   - Verify local: `mongod --version`

3. **Git** (optional, if cloning)

---

### 📦 Step-by-Step Setup

#### Step 1 – Extract the ZIP
```
Unzip KrishiMitra.zip to any folder (e.g., Desktop/KrishiMitra)
```

#### Step 2 – Setup Backend
```bash
# Open terminal, go to backend folder
cd KrishiMitra/backend

# Install dependencies
npm install

# (Optional) Seed demo data
npm run seed
```

#### Step 3 – Setup Frontend
```bash
# Open a NEW terminal tab
cd KrishiMitra/frontend

# Install dependencies
npm install
```

#### Step 4 – Start MongoDB
```bash
# If using local MongoDB:
mongod

# OR if using MongoDB Atlas, update MONGODB_URI in backend/.env
```

#### Step 5 – Start Backend Server
```bash
cd KrishiMitra/backend
npm run dev
# Server starts at http://localhost:5000
```

#### Step 6 – Start Frontend
```bash
cd KrishiMitra/frontend
npm start
# App opens at http://localhost:3000
```

---

### 🎯 Demo Login (after seeding)
```
Email:    demo@krishimitra.in
Password: demo123
```

---

## 🌐 Pages & Features

| Page | URL | Features |
|------|-----|----------|
| Landing | / | Hero, features, stats |
| Login | /login | JWT auth, demo login |
| Register | /register | 3-step wizard |
| Dashboard | /dashboard | Stats, weather, market snapshot |
| Crops | /crops | Add/edit/delete crops, growth tracker |
| Weather | /weather | 7-day forecast, farming advice |
| Market | /market | Live mandi prices, price trend chart |
| Advisory | /advisory | Pest/disease alerts by category |
| Soil Health | /soil | Soil test logs, radar chart |
| Community | /community | Posts, likes, comments |
| Profile | /profile | Update farm & personal details |

---

## ⚙️ Environment Variables (backend/.env)

```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/krishimitra
JWT_SECRET=your_secret_key_here
OPENWEATHER_API_KEY=your_key_here   # optional, works without it (mock data)
NODE_ENV=development
```

---

## 🗒 Notes

- Weather works with **mock data** by default — no API key needed
- Market prices are **simulated** (real data needs government API integration)
- For **real weather**, get a free key from https://openweathermap.org/api
- App is **mobile responsive** out of the box

---

Made with ❤️ for Indian Farmers | KrishiMitra 2024
