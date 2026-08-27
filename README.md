# 🛡️ Sentinel AI

## AI-Powered Cybercrime Complaint Management System

<div align="center">

[!\[License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[!\[Hackathon Winner](https://img.shields.io/badge/🏆%202nd%20Rank-INDORE%20TECH%20HACKATHON%202025-blue)](.)

> ### 🚀 \*\*"Empowering Citizens. Protecting Communities. Detecting Threats."\*\*
</div>

\---

## ⭐ Overview

**Sentinel AI** is a comprehensive cybercrime management platform featuring:

* 🎯 AI-powered complaint management \& analysis
* 🤖 5 intelligent detection modules (malicious text, call scams, summarization, similarity, biometrics)
* 🔐 Enterprise security (CAPTCHA, typing biometrics, VPN detection)
* 📱 Real-time notifications \& tracking
* 🌐 Production-ready with Docker \& AWS deployment

\---

## 🌍 Problem Statement

Cybercrime has become one of the fastest-growing threats in the digital age, with citizens frequently encountering phishing attacks, scam calls, financial fraud, identity theft, and social engineering campaigns.

Traditional reporting systems often suffer from:

* Delayed response times
* Manual complaint triage
* Fragmented evidence management
* Limited threat intelligence capabilities
* Poor citizen engagement and accessibility

Sentinel AI addresses these challenges by combining artificial intelligence, cybersecurity analytics, and citizen-centric design into a unified platform capable of detecting, analyzing, and managing cybercrime incidents at scale.

\---

## 🎯 Core Features

### Citizens

|Feature|Purpose|
|-|-|
|🚨 Register Complaint|Submit reports with multimedia evidence|
|🔍 Scam Detector|Verify suspicious calls \& messages|
|💬 AI Chatbot|24/7 cybercrime guidance|
|📱 Track Status|Real-time complaint updates|
|🔔 Nudge System|Request urgent attention|

### Administrators

|Feature|Purpose|
|-|-|
|📊 Analytics Dashboard|Real-time complaint statistics|
|🧠 AI Analysis|Auto-summarization \& severity scoring|
|🔗 Duplicate Detection|Find related complaints|
|👀 Security Monitoring|Login anomaly \& VPN detection|
|🔒 Audit Trail|Secure deletion with verification|

\---

## 🌐 Project Modules

### 1\. **Web Sentinel** - Phishing Detection Chrome Extension

Real-time phishing detection using 16 heuristics and ML classifier.

```
Phishing Detection Chrome Extension/Web-Sentinel/
├── manifest.json
├── popup.html \& popup.js
├── content.js (page scanner)
└── MODEL.md (ML details)
```

**Features:** Auto-scan on page load, heuristic-based detection, reputable-root allowlist

### 2\. **Sentinel AI Core** - Main Platform

Complete cybercrime complaint system with AI modules.

```
api/                    # FastAPI backend
frontend-react/         # React + TypeScript frontend
summarizer/             # Complaint analysis
call\_scam\_detector/     # Audio analysis
IAP\_AI\_Malicious\_Detector/  # Text analysis
chatbot/                # RAG-based assistant
TypingIPVPNDetector/    # Security verification
```

\---

## 🚀 Quick Start

### Prerequisites

```bash
Python 3.8+  |  Node.js 16+  |  Docker (optional)
```

### Backend Setup

```bash
cd d:\\Complete\_package\\abc
python -m venv .venv
.venv\\Scripts\\activate
pip install -r requirements.txt
python -m uvicorn api.main:app --reload
```

**API runs on:** http://localhost:8000/docs

### Frontend Setup

```bash
cd frontend-react
npm install
npm run dev
```

**Frontend runs on:** http://localhost:5173

### Chrome Extension Setup

```
1. Open chrome://extensions
2. Enable Developer mode
3. Click "Load unpacked" → Select Phishing Detection Chrome Extension/Web-Sentinel/
```

\---

## 🏗️ Architecture

### Backend Stack

* **Framework:** FastAPI (Python)
* **Database:** SQLite
* **Auth:** JWT + CAPTCHA + Biometrics
* **APIs:** Groq LLM, Tavily Search

### Frontend Stack

* **Framework:** React 18 + TypeScript
* **Build:** Vite
* **Styling:** CSS

### AI/ML Capabilities

* **Text Analysis:** Groq LLM for malicious content detection
* **Audio Analysis:** Vosk speech-to-text + scam classification
* **Summarization:** Extractive + abstractive summarization
* **Similarity:** FAISS vector search for duplicate detection
* **Biometrics:** Typing pattern analysis for anomaly detection

\---

## 📦 Project Structure

```
.
├── README.md                              # Main documentation
├── LICENSE                                # MIT License
├── CONTRIBUTING.md                        # Guidelines
├── docker-compose.yml                     # Docker setup
├── requirements.txt                       # Python dependencies
│
├── api/                                   # FastAPI Backend
│   ├── main.py                            # Main app
│   ├── database.py                        # Database models
│   ├── similarity.py                      # NLP matching
│   └── uploads/                           # User evidence
│
├── frontend-react/                        # React Frontend
│   ├── src/pages/                         # Page components
│   ├── src/components/                    # Reusable components
│   └── package.json
│
├── Phishing Detection Chrome Extension/   # Chrome Extension
│   └── Web-Sentinel/
│       ├── manifest.json
│       ├── popup.html
│       └── content.js
│
├── call\_scam\_detector/                    # Audio analysis
├── IAP\_AI\_Malicious\_Detector/             # Text analysis
├── TypingIPVPNDetector/                   # Security module
├── chatbot/                               # AI assistant
├── summarizer/                            # Complaint analysis
│
└── docs/                                  # Archived documentation
```

\---

## 🔒 Security Features

* **CAPTCHA Verification** - 6-character alphanumeric
* **Typing Biometrics** - WPM analysis + anomaly detection
* **IP/VPN Detection** - Geolocation + proxy identification
* **Login Monitoring** - Complete audit trail
* **Password Hashing** - bcrypt with salt
* **Data Encryption** - Evidence file protection

\---

## 🤖 AI/ML Modules

### Complaint Summarization

* Multi-format support (PDF, images, audio, video)
* Automatic evidence extraction
* Severity classification (1-5 score)

### Malicious Text Detection

* Input: Chat messages, emails, SMS
* Detection: Phishing, social engineering, scareware
* Output: Threat score (0-100)
* **Accuracy: 94%**

### Call Scam Detection

* Audio processing: Vosk (English \& Hindi)
* Classification: Safe → Scam
* Processing time: < 5 seconds

### Duplicate Detection

* Technology: Sentence Transformers + FAISS
* Performance: O(1) lookup
* Identifies related fraud patterns

\---

## 🧠 AI Innovation Highlights

Sentinel AI integrates multiple specialized AI systems working collaboratively to provide comprehensive threat analysis:

### Multimodal Intelligence

The platform processes multiple forms of evidence including:

* Text messages
* Emails
* Audio recordings
* PDFs
* Images
* Videos

allowing investigators to build richer contextual understanding of reported incidents.

### Retrieval-Augmented Assistance

The cybercrime chatbot leverages retrieval-augmented generation (RAG) techniques to provide grounded and context-aware responses for citizens seeking guidance regarding scams, fraud, and cybersecurity best practices.

### Explainable Threat Scoring

Instead of providing opaque predictions, Sentinel AI generates interpretable threat assessments that help both citizens and administrators understand the reasoning behind classifications and severity scores.

\---

## 🐳 Deployment

### Local Docker

```bash
docker-compose up -d --build
```

Access: http://localhost

### AWS EC2 (Free Tier)

```bash
# Launch Ubuntu 22.04 t2.micro instance
ssh -i key.pem ubuntu@YOUR\_IP
curl -fsSL https://get.docker.com | sh
docker-compose up -d --build
```

Access: http://YOUR\_EC2\_IP

\---

## 📊 Platform Impact

### Key Capabilities

|Capability|Description|
|-|-|
|Complaint Intelligence|Automated complaint summarization and prioritization|
|Scam Detection|Text and voice-based fraud analysis|
|Phishing Prevention|Browser-based website threat detection|
|Threat Correlation|Duplicate fraud pattern identification|
|Security Monitoring|Behavioral and network anomaly detection|
|Citizen Assistance|AI-powered cybercrime support system|

### Design Goals

* Improve cybercrime reporting accessibility
* Reduce complaint processing overhead
* Accelerate fraud pattern discovery
* Enhance citizen awareness
* Support scalable smart-city cybersecurity initiatives

\---<div align="center">

Made with ❤️ by Sentinel AI Team

</div>

