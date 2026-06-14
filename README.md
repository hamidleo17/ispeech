# AuraSpeech: Premium Text-to-Speech Engine

A complete, production-ready text-to-speech engine. Crafted with an elegant Apple-style glassmorphism interface, offline fallbacks, and multi-view policies, optimization is baked-in for high-fidelity audio synthesis.

## 🌟 Key Features

1. **AuraSpeech Synthesis Interface**: Frosted transparent glass layout complete with character parameters, real-time counters, TXT uploads (drag & drop & selector), speed sliders, and pitch toggles.
2. **Dual Acoustic Synthesis Engines**:
   - **Google Cloud TTS (Premium AI)**: Features standard and Neural2 high-fidelity voices (Emma, Mia, Sofia, Sakura, Chloe...) for realistic stresses, accent variants, and lifelike breathing models.
   - **Local Browser Synthesis (100% Free Fallback)**: Runs offline on device-level systems, bypassing quotas and keys instantly if required.
3. **Advanced Sound wave Animation**: Interactive 15-bar CSS visualizer dancing in real-time when audio plays.
4. **Local Historic Backups**: Saves up to 5 of your latest generation queries inside `localStorage` for instant load and repeat plays offline.
5. **Ethical Non-Intrusive Ad Units**: Centered banner, desktop sidebars, and footer sections pre-configured with Google AdSense slot anchors.
6. **Built-in Smart Cache Layer**: Server-level parameters hashing retains compiled MP3 files for 1 hour, saving API quotas and avoiding excessive calls.

## 🛠️ Setup Instructions

Ensure Node JS (v18+) is installed on your local environment.

### 1. Installation

Install necessary packages and run the application:

```bash
# Install dependencies
npm install

# Start full-stack local server
npm run dev
```

The application will launch on your native browser at `http://localhost:3000`.

### 2. Environment Configurations

Define the following parameters inside your `.env` file at root level:

```env
# Google Cloud Platform TTS API Key OR standard Gemini key
GOOGLE_API_KEY="your_google_cloud_api_key_here"

# (Optional backup)
GEMINI_API_KEY="your_gemini_api_key_here"
```

### 3. Build & Production Deployment

To package the front and backends for production environments:

```bash
# Build client bundle & package server.ts into dist/server.cjs
npm run build

# Start the compiled bundle CJS executable
npm run start
```

## 📈 Ethical AdSense Integration

Uncomment the Google AdSense code injection blocks located inside `src/components/AdSlot.tsx` once your AdSense profile is certified to place active ads.
