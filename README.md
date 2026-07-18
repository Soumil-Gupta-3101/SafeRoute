# SafeRoute 🛡️
**Women's Safety Navigator** — *Navigate Smart. Stay Safe. Even Offline.*

SafeRoute helps women navigate Indian cities safely by comparing a **Safe Route** vs the **Fastest Route** using real incident data and time-of-day risk mapping.

---

## Features
- 🗺️ Incident heatmap with time-of-day slider
- 🔀 Safe vs Fastest route comparison with safety score
- 🆘 One-tap SOS — sends SMS to trusted contacts even offline
- 👥 Crowdsourced incident reporting + community validation
- 📵 PWA — installs on phone, works without internet

## Tech Stack
- **Frontend** — React.js, Vite, Leaflet.js
- **Backend** — Node.js, Express.js, MongoDB
- **Routing** — OSRM (free), Nominatim geocoding
- **SMS** — Fast2SMS
- **Real-time** — Socket.io

## Setup

```bash
# Backend
cd server
npm install
npm run seed     # seed 150 Chandigarh incidents
npm run dev      # runs on http://localhost:5000

# Frontend
cd client
npm install
npm run dev      # runs on http://localhost:5173
```

**server/.env**
```
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
FAST2SMS_API_KEY=your_fast2sms_key
CLIENT_URL=http://localhost:5173
PORT=5000
```
