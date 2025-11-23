# Zenix Travel Companion

Your smart AI guide for stress-free travel — a lightweight Gradio app that helps you plan, explore, and enjoy trips with personalized suggestions.

[![Hugging Face Space](https://img.shields.io/badge/Hugging%20Face-Space-orange?logo=huggingface)](https://huggingface.co/spaces/TayyabKhalid/Zenix_Travel_Companion) [![Python](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/)

Live demo: [https://huggingface.co/spaces/TayyabKhalid/Zenix_Travel_Companion](https://huggingface.co/spaces/TayyabKhalid/Zenix_Travel_Companion)

Quick summary
- AI-driven itinerary generation tailored by destination, trip length, and traveler style
- Packing checklists and travel tips
- Local recommendations and safety reminders
- Mobile-friendly Gradio UI for fast exploration

Why this repo
This repository contains the code for Zenix Travel Companion — a user-friendly Gradio app ready to run locally or hosted on Hugging Face Spaces. 

Features
- Generate sample itineraries and day-by-day plans
- Packing list generation (by weather, trip type)
- Local tips (transport, tipping, safety)
- Quick Q&A about travel planning

Run locally
1. Clone
   
```bash
git clone https://github.com/Holy-Warrior/Zenix_Travel_Companion.git
cd Zenix_Travel_Companion
```

2. Environment
```bash
python -m venv .venv
source .venv/bin/activate   # macOS / Linux
.venv\Scripts\activate      # Windows
```

3. Install
```bash
pip install -r requirements.txt
```

4. Start
```bash
python app.py
Open http://localhost:7860 in your browser (default Gradio port)
```

