# Agnivani - Backend API 🌾

[![Node.js](https://img.shields.io/badge/Node.js-v18+-green.svg)](https://nodejs.org/)
[![Express.js](https://img.shields.io/badge/Express.js-v4+-blue.svg)](https://expressjs.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-v6+-green.svg)](https://mongodb.com/)

Agnivani is a professional farming advisory platform. This repository contains the backend API services built with Node.js, Express, and MongoDB. It provides authentication, crop recommendations, weather data integration, AI chatbots, and voice synthesis capabilities.

## 🚀 Features

- **Robust Authentication**: Secure OTP-based authentication and JWT authorization.
- **RESTful Architecture**: Clean, scalable, and well-structured API endpoints.
- **AI Integration**: AI-powered crop doctor integration.
- **Location Services**: Geolocation-based state and weather fetching.
- **Text-to-Speech (TTS)**: ElevenLabs API integration for voice-assisted farming guidance.
- **Crop Database Management**: Manage and retrieve state-specific crop data.

## 📁 Directory Structure

```text
├── functions/      # Core business logic and controllers
├── middlewares/    # Custom middlewares (e.g., JWT Authentication)
├── utils/          # Utility functions and database connections
├── index.js        # Application entry point & route definitions
├── package.json    # Project dependencies
└── .env.example    # Example environment variables
```

## 🛠️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone <repository_url>
   cd Hackspire-2025-backend
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure Environment Variables**
   Copy the example environment file and fill in your credentials.
   ```bash
   cp .env.example .env
   ```

   **Required Variables:**
   - `PORT`: Port to run the server (Default: 4000)
   - `MONGODB_URI`: MongoDB connection string
   - `JWT_SECRET`: Secret key for signing JWTs
   - `LOCATION_API_KEY`: API key for location services
   - `ELEVENLABS_API_KEY`: ElevenLabs API key for TTS
   - `EMAIL_OTP_SENDER_API`: API for sending OTPs

4. **Start the Development Server**
   ```bash
   npm run dev
   ```

## 🛣️ API Endpoints

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| GET | `/` | Health check | No |
| POST | `/api/auth/send-otp` | Send login OTP | No |
| POST | `/api/auth/verify-otp` | Verify OTP & Login | No |
| GET | `/api/auth/me` | Get current user info | No |
| GET | `/crops/get-all` | Get all crops | Yes |
| POST | `/crops/create-new` | Add new crop | Yes |
| GET | `/indian-states/get-all`| Get all states data | Yes |
| POST | `/apis/text-to-speech` | Generate speech audio| No |

## 🛡️ Security
This API uses **JWT (JSON Web Tokens)** for securing protected routes. Pass the token as a Bearer token in the `Authorization` header.

## 📜 License
This project is licensed under the ISC License.
