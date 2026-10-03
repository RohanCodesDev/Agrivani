# Agnivani - Frontend Application 🌾

[![Next.js](https://img.shields.io/badge/Next.js-v14+-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-v18+-blue.svg)](https://reactjs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-v3+-38B2AC.svg)](https://tailwindcss.com/)

Welcome to the **Agnivani** frontend application! This is a modern, responsive, and highly interactive farming advisory platform built with Next.js (Pages Router), React, and Tailwind CSS. It is designed to assist farmers by providing real-time crop recommendations, AI-powered chatbots, live weather updates, and multilingual text-to-speech functionality.

## ✨ Key Features

- **Crop Doctor (AI Integration)**: Direct integration with Google Gemini for image-based crop disease diagnosis and a conversational AI chatbot.
- **Multilingual Voice Assistant**: Text-to-speech capabilities leveraging ElevenLabs APIs for accessibility.
- **Real-time Weather Forecast**: Integrates with OpenWeatherMap API for accurate local weather and agricultural forecasting.
- **Progressive Web App (PWA) Ready**: Built with mobile-first principles for seamless usage in the field.
- **Authentication**: JWT-based login and signup flows with OTP support.
- **Modern UI/UX**: Built with Radix UI components, Tailwind CSS, and Framer Motion (tw-animate-css) for smooth, premium animations and accessibility.

## 📁 Directory Architecture

```text
├── src/
│   ├── components/    # Reusable UI components (Weather, Chatbot, Dialogs, etc.)
│   ├── contexts/      # React Contexts for global state management
│   ├── pages/         # Next.js Pages routing (includes API routes if any)
│   ├── styles/        # Global CSS and Tailwind directives
│   └── lib/           # Utility functions and shared helpers
├── public/            # Static assets (images, fonts, icons)
├── package.json       # Dependencies and scripts
└── .env.example       # Example configuration variables
```

## 🛠️ Getting Started

1. **Clone the repository**
   ```bash
   git clone <repository_url>
   cd Hackspire-2025-frontend_new
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure Environment Variables**
   Create a `.env.local` file by copying the provided example:
   ```bash
   cp .env.example .env.local
   ```
   **Required Variables:**
   - `NEXT_PUBLIC_BASE_URL`: URL of the backend API (e.g., `http://localhost:4000`)
   - `NEXT_PUBLIC_YOUR_API_KEY`: OpenWeatherMap API Key
   - `NEXT_PUBLIC_GEMINI_API_KEY`: Google Gemini API Key

4. **Run the Development Server**
   ```bash
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🌍 Supported Integrations
- **Google Gemini**: For AI crop advisory.
- **OpenWeatherMap**: For hyper-local weather alerts.
- **ElevenLabs**: For lifelike text-to-speech rendering in Indian languages.

## 🤝 Contribution Guidelines
When contributing to this repository, please ensure that you follow the established design systems (Tailwind + Radix) and that all new components are responsive.

## 📜 License
This project is proprietary and confidential for Hackspire 2025.
