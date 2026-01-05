# 🤖 Project Penny: AI-Powered Financial Fraud Detection

**🏆 Winner: Best Project — USC MAIA Demo Day (Fall 2025)** Recognised by a judging panel of engineers from Netflix and Google for technical rigour, market viability, and tangible impact on senior digital safety.

---

## 📌 Project Overview
Project Penny is a comprehensive hardware-software ecosystem designed to protect elderly residents in nursing homes from financial fraud. By combining real-time audio processing with machine learning classification, Penny detects scam indicators in VOIP calls and instantly alerts caregivers via a mobile dashboard.

* **Organisation:** Marshall AI Association (MAIA) — Finance Department, USC
* **Role:** Audio Processing Engineer & iOS Frontend Developer
* **Stack:** Python, Raspberry Pi 5, React Native (Expo), DistilBERT, Supabase, VOSK

---

## ⚠️ The Problem
Approximately **$28.3 billion** is stolen annually from Americans over the age of 60 via financial fraud. Seniors in assisted living facilities are primary targets for sophisticated scams that exploit cognitive vulnerabilities.

---

## 💡 The Solution
Penny provides a multi-layered defence system:
* **Hardware Monitoring:** A Raspberry Pi-powered device monitors VOIP streams for high-signal scam indicators.
* **Immediate Feedback:** Physical GPIO stoplight indicators provide visual status for residents.
* **Caregiver Triage:** A React Native iOS application provides nursing home staff with real-time push notifications and a facility-wide risk dashboard.



---

## 🛠 Technical Contributions

### 1. Audio Processing Pipeline (`backend/`)
I engineered the system to ensure high-fidelity data capture for ML inference while maintaining strict resident privacy.
* **Signal Processing:** Implemented 300-3400 Hz bandpass filters using `scipy` to isolate human speech.
* **Performance:** Architected a producer-consumer threading pattern with thread-safe queues to maintain <20ms latency.
* **Privacy-First STT:** Integrated **VOSK** for local Speech-to-Text transcription, ensuring no private audio data leaves the local network.

### 2. iOS Mobile Application (`frontend/`)
Co-developed a 7-screen caregiver interface focused on high-speed monitoring and triage.
* **Live Alerts:** Colour-coded risk levels (High, Medium, Low) with instant push notifications.
* **Facility Dashboard:** Overview of 40+ residents per facility, active alerts, and weekly safety summaries.
* **Platform:** Built using React Native and Expo Go for rapid deployment to nursing home staff devices.

### 3. Cloud Infrastructure (`supabase/`)
* **Real-time Sync:** Integrated Supabase for remote ML inference and data storage.
* **Infrastructure as Code:** Managed Supabase integrations and automated workflows via GitHub Actions.

---

## 📂 Repository Structure
* **`backend/`**: Python core logic for signal processing and speech-to-text.
* **`frontend/`**: React Native (Expo) source code for the caregiver mobile application.
* **`supabase/`**: Database schema, edge functions, and cloud integrations.
* **`src/`**: Shared source components and utility functions.
* **`MAIA_PENNY_PROJECT.pdf`**: Full technical case study and pitch deck.


---

## 🔗 Resources
* [Demo Day Slide Deck](https://drive.google.com/file/d/1mkdHl195nxZl4Q1QlQAQ8YxHY1EbaRjb/view?usp=sharing)
* [Main Portfolio Hub](https://github.com/omatasie/oma_tasie_portfolio)

---

*Developed by Oma Tasie-Amadi and Team @ USC Marshall AI Association. Because Every Penny Matters.*
