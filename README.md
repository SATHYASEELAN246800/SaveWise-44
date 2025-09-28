# SaveWise — AI-Powered Multi-Currency Savings & Tracking

[![Project Status](https://img.shields.io/badge/status-Active-brightgreen)](https://app.base44.com/apps/68cc18d7d243ad4e9e5cea1c/editor/preview)
[![License](https://img.shields.io/badge/license-MIT-blue)]()

---

## 📌 Project Overview

**SaveWise** is a professional, AI-powered multi-currency savings and tracking platform built with **Base44 AI**.  
It empowers users to **track, predict, and optimize savings**, providing intelligent recommendations and AI reasoning through a contextual chatbot.

- **Target Users:** Students, young professionals, travelers, and families.  
- **Key Goal:** Turn personal finance management into a seamless, futuristic, and AI-driven experience.

---

## ⚡ Features

### Core Functionality
- 💰 **Multi-Currency Wallets**: Track and manage multiple wallets in INR, USD, EUR, etc., with base-currency aggregation (₹ default).  
- 📊 **Smart Insights Dashboard**: Pie charts, line graphs, and heatmaps showing savings, expenses, and category breakdown.  
- 🎯 **Goal-Oriented Saving**: Set goals, track progress, and receive AI-powered suggestions to stay on target.  
- 🔔 **Smart Notifications**: Weekly summaries, overspend alerts, and goal reminders.  
- 🤖 **AI Assistant**: Chatbot using Groq LLM for reasoning on your financial data, answering queries, and forecasting.

### AI & Smart Features
- 💡 **Budget Healer**: Automatically adjusts budgets and provides cost-saving suggestions.  
- 📈 **Future Forecasting**: Predicts savings and expenses over 1–6 months using ML models.  
- 😊 **Emotion Insights**: Correlates mood with spending patterns.  
- 🌍 **Currency Volatility Guard**: Advises when to convert or hold currencies.  
- 💹 **Micro-Investment Suggestions**: Simulates safe investment options with predicted returns.  
- 🔄 **Auto Round-Up Savings**: Small change from transactions automatically saved.

### User Engagement
- 🏅 Gamification: Badges, streaks, and leaderboards.  
- 👨‍👩‍👧‍👦 Savings Circles: Group goals and shared contributions.  
- 🎙 Voice Assistant: Add transactions and goals via voice commands (Web Speech API + serverless fallback).  
- 🌐 Offline Mode + Smart Sync (PWA + IndexedDB).  

### Utilities
- CSV/PDF export & import for transactions and statements.  
- GDPR-style data export and deletion.  
- Admin dashboard for managing demo data and global settings.

---

## ⚙️ Tech Stack

### Frontend & Web (Base44 Powered)
- Base44 AI (App Generation Platform)  
- Next.js (App Router)  
- Tailwind CSS + shadcn/ui (UI styling & components)  
- Framer Motion (animations & micro-interactions)  
- Recharts / D3.js (financial charts)  
- PWA + IndexedDB (offline mode & smart sync)  
- Glassmorphism UI (professional, futuristic design)  

### Backend & Infrastructure
- Base44 Serverless Functions  
- MongoDB Atlas / Supabase (database options)  
- Redis Caching for fast insights  
- CSV/PDF Reports (import/export + statements)  
- Web Push + Email Alerts (notifications, weekly summaries)  

### AI & Intelligence Layer
- **Groq API (LLM)** — lightning-fast reasoning chatbot  
- **LangChain.js** — orchestrate LLM reasoning + structured data  
- TensorFlow.js / PyTorch — savings forecasting & simulations  
- scikit-learn + Prophet — regression & future predictions  
- ARIMA Models — expense/savings volatility guard  
- Hugging Face Transformers — embeddings & mood correlation  
- Vector DB (Pinecone / Weaviate) — RAG over historical user financial data  
- spaCy + NLTK — NLP & sentiment analysis  
- Whisper ASR — voice-enabled transaction input  
- Rule-based deterministic AI fallbacks  

### Security & Auth
- JWT-based sessions & refresh tokens  
- OAuth 2.0 (Google Sign-in)  
- Bcrypt / Argon2 for password hashing  
- Rate-limiting + Input validation  

### User Experience & Engagement
- Gamification (badges, streaks, leaderboards)  
- Savings Circles (group goals)  
- Accessible design (WCAG 2.1)  
- SEO optimized + responsive layout  

---

## 🗂️ Data Models

### User
```json
{
  "_id": "ObjectId",
  "name": "string",
  "email": "string",
  "passwordHash": "string",
  "wallets": ["ObjectId"],
  "circles": ["ObjectId"],
  "preferences": {"baseCurrency": "INR", "theme": "dark", "timezone": "Asia/Kolkata"}
}
