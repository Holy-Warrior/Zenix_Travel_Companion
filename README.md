# Zenix Travel Companion

Your smart AI guide for stress-free travel — a lightweight Gradio app that helps you plan, explore, and enjoy trips with personalized suggestions.

[![Hugging Face Space](https://img.shields.io/badge/Hugging%20Face-Space-orange?logo=huggingface)](https://huggingface.co/spaces/Holy-Warrior/Zenix_Travel_Companion) [![Python](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/)

Live demo: https://huggingface.co/spaces/Holy-Warrior/Zenix_Travel_Companion

Quick summary
- AI-driven itinerary generation tailored by destination, trip length, and traveler style
- Packing checklists and travel tips
- Local recommendations and safety reminders
- Mobile-friendly Gradio UI for fast exploration

Why this repo
This repository contains the code for Zenix Travel Companion — a user-friendly Gradio app ready to run locally or hosted on Hugging Face Spaces. The README and docs include instructions to also publish a small GitHub Pages site that embeds the live Hugging Face Space so visitors can find and open the app easily.

Features
- Generate sample itineraries and day-by-day plans
- Packing list generation (by weather, trip type)
- Local tips (transport, tipping, safety)
- Quick Q&A about travel planning

Run locally
1. Clone
   git clone https://github.com/Holy-Warrior/Zenix_Travel_Companion.git
   cd Zenix_Travel_Companion

2. Environment
   python -m venv .venv
   source .venv/bin/activate   # macOS / Linux
   .venv\Scripts\activate      # Windows

3. Install
   pip install -r requirements.txt

4. Start
   python app.py
   Open http://localhost:7860 in your browser (default Gradio port)

Deployment / Hosting options
- Hugging Face Spaces (recommended for Gradio apps) — already live.
- GitHub Pages — serve a docs/ folder as a static site that embeds the Hugging Face Space (instructions below).
- Other hosts (Render, Railway, Replit) for running the app as a process.

Make it available on GitHub Pages (what I prepared)
- I included a small docs/index.html that embeds your Hugging Face Space in an iframe and provides a fallback link if embedding is blocked.
- To publish:
  1. Add docs/index.html to the repo (file provided below).
  2. Commit & push to main (or a branch and open a PR).
  3. Go to the repository Settings → Pages.
  4. Under "Build and deployment", set Source to: Branch: main, Folder: /docs, Save.
  5. After a few minutes your site will be at:
     https://Holy-Warrior.github.io/Zenix_Travel_Companion/

Note on embedding
- Some sites disable framing via headers (X-Frame-Options or Content-Security-Policy). If the Hugging Face Space blocks framing, the iframe will show a notice and users can use the prominent link to open the Space in a new tab.

docs/index.html (included in this repo to enable Pages) — see the file block below.

Contributing
Contributions are welcome. Please open an issue for ideas or bugs, or submit a PR for small fixes. Suggested next contributions:
- Add a LICENSE file (MIT, Apache-2.0, or GPL—tell me if you want one added)
- Add screenshots and a short demo GIF
- Add tests and CI (GitHub Actions) if you want automated checks on PRs

Suggested commit to add these docs
git checkout -b add-readme-and-pages
git add README.md docs/index.html
git commit -m "Improve README and add GitHub Pages docs with embedded Space"
git push -u origin add-readme-and-pages
Open a PR or merge to main.

Troubleshooting
- If the app doesn't start, ensure dependencies in requirements.txt match your environment.
- If GitHub Pages doesn't show, double-check Settings → Pages configuration and that docs/index.html exists on the selected branch.
- If the iframe appears blank, try the direct link to Hugging Face Space — embedding may be blocked.

License
Add a LICENSE file to clarify reuse. If you tell me which license you prefer, I can create the file for you.

Contact
Created and maintained by Holy-Warrior. For help or changes, open an issue in this repo.
