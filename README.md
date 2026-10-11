🌍 AI Travel Agent – Multilingual Audio Guide

An AI-powered travel guide that generates informative descriptions of tourist destinations and converts them into audio guides in multiple languages.

🚀 Live Demo

Live Website: https://travel-guide-1-up82.onrender.com/

✨ Features

- Destination Exploration: Explore popular tourist destinations.
- AI-Powered Descriptions: Generate destination information using Google Gemini AI.
- Summary and Detailed Modes: Choose between a concise summary and a detailed explanation.
- Multilingual Support: Generate guides in English, Hindi, Tamil, and Telugu.
- AI Voice Generation: Convert generated descriptions into audio using Murf AI.
- Voice Selection: Choose between male and female voices.
- Audio Playback: Listen to generated guides directly on the website.

🛠️ Technologies Used

Frontend

- HTML
- CSS
- JavaScript

Backend

- Python
- Flask
- Flask-CORS

AI Services

- Google Gemini API
- Murf AI Text-to-Speech API

Deployment

- Render Static Site for the frontend
- Render Web Service for the backend

📁 Project Structure

Travel_agent/
├── Backend/
│   ├── app.py
│   └── requirements.txt
├── Frontend/
│   ├── index.html
│   └── index.js
└── README.md

⚙️ Setup Instructions

Follow these steps to run the project locally.

Prerequisites

Install:

- Python 3.10 or later
- Git
- A modern web browser

You will also need API keys for Google Gemini and Murf AI.

1. Clone the Repository

git clone https://github.com/jyothirmaeenuthalapati/travel_guide.git
cd Travel_agent


2. Set Up the Backend

Navigate to the backend directory:

cd Backend

Create a virtual environment:

python -m venv venv

Activate it on Windows:

venv\Scripts\activate

On macOS or Linux:

source venv/bin/activate

Install the dependencies:

pip install -r requirements.txt

3. Configure API Keys

Create a ".env" file inside the "Backend" directory.

Add your own API keys:

GEMINI_API_KEY=your_gemini_api_key
MURF_API_KEY=your_murf_api_key

Replace the placeholder values with your actual API keys.

Security: Never commit your ".env" file or publish your API keys in a public repository.

4. Start the Backend

From the "Backend" directory, run:

python app.py

The backend will run locally at:

"http://127.0.0.1:5000"

The API endpoint used to generate audio guides is:

"POST /generate-audio-guide"

5. Configure and Run the Frontend

Open "Frontend/index.js" and configure the API URL to point to the backend you want to use.

For local development:

const GENERATE_AUDIO_GUIDE_API_URL =
  "http://127.0.0.1:5000/generate-audio-guide";

Save the file.

Run the frontend using a local development server, such as the Live Server extension in Visual Studio Code, and open the provided local website address in your browser.

Keep the Flask backend running while using the application.

🌐 Deployment

The application is deployed on Render as two separate services.

- Frontend: https://travel-agent-frontend-3z38.onrender.com
- Backend: https://travel-agent-zgxw.onrender.com

The frontend communicates with the deployed backend through HTTP requests.

For local development, use the local API URL shown in the setup instructions. For the deployed website, use the deployed backend API URL.

🔑 API Requirements

The application requires:

- Google Gemini API for generating destination descriptions.
- Murf AI API for generating audio.

API availability, usage limits, and charges depend on the providers' current plans and policies.

🎯 Project Objective

The objective of this project is to make destination exploration more interactive and accessible by combining generative AI with multilingual audio guides.

👩‍💻 Author

Developed as an AI-powered travel assistance project.
