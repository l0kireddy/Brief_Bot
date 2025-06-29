# 🤖 BriefBot – AI-Powered Meeting Summarizer

BriefBot is an AI tool that turns long meeting recordings into concise summaries and task lists. It combines Whisper for transcription and IBM watsonx Granite models for intelligent summarization.

📂 Project Structure

Brief_Bot/
│
├── Working Model/                # Full stack working web app
│   ├── backend/                  # Flask + Whisper + Granite API
│   │   ├── app.py
│   │   └── requirments.txt
│   └── frontend/                 # React frontend (Vite)
│       ├── public/
│       ├── src/
│       └── README.md
│
├── Working Prototype/           # Lightweight prototype versions
│   ├── Brief_Bot(working_prototype).ipynb   # Colab-compatible notebook
│   └── brief_bot(working_prototype).py      # Script version (no server)
│
├── LICENSE
└── README.md                    # You're here

⚠️ Important

🔐 You have to change the api_key and project_id in all backend and prototype files.These credentials are required to connect to IBM watsonx.ai and will not work unless replaced with your own.

🚀 Working Model (Full Stack App)

📆 Backend Setup (Flask + Whisper + Granite)

Navigate to Working Model/backend/

Install Python dependencies:

pip install -r requirments.txt

Update the following in app.py:

api_key = "your_ibm_api_key_here"        # 🔥 Must replace
project_id = "your_project_id_here"      # 🔥 Must replace

Start the Flask server:

python app.py

🌐 Frontend Setup (React + Vite)

Navigate to Working Model/frontend/

Install dependencies:

npm install

Run the frontend:

npm run dev

Visit http://localhost:5173 to use BriefBot locally

🥪 Working Prototype (No Server Required)

✅ Option 1: Run in Google Colab

Open Brief_Bot(working_prototype).ipynb

Upload a video/audio file

It transcribes using Whisper and summarizes using IBM Granite

Perfect for quick demos

✅ Option 2: Python Script

Run brief_bot(working_prototype).py using:

python brief_bot(working_prototype).py

Edit the script to set your IBM API key, and upload a file for offline use

💠 Dependencies

Python 3.9+

Whisper (openai/whisper)

ffmpeg

Flask

ibm-watsonx-ai

React (Vite-based frontend)

📸 UI Demo

Upload & Analyze

AI Summary Output





🧠 Powered By

🗣️ Whisper – Speech-to-text by OpenAI

🤠 IBM Granite – Foundation models via watsonx.ai

⚛️ React + Flask – Full stack for real-time app

🛡️ License

MIT License © 2025 l0kireddy

🤛 Support

Raise an issue or open a discussion if you get stuck — or ping @l0kireddy on GitHub.
