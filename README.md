# Campus Sarthi Chatbot

[![Python Version](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Issues](https://img.shields.io/github/issues/sonali19705/CampusSarthi-chatbot)](https://github.com/sonali19705/CampusSarthi-chatbot/issues)

---

## Overview
Campus Sarthi is a multilingual AI-powered chatbot designed to assist students and faculty with college-related queries.
It provides instant, accurate responses about courses, faculty details, exams, library services, and general campus information.

The system supports multiple languages, making it inclusive and user-friendly for a diverse audience.

---

## Features
🌐 Multilingual support (English, Hindi, Gujarati)
💬 Real-time chatbot interaction
📚 FAQ-based and semantic search responses
🧠 AI-powered response matching using vector database
🛠️ Admin panel to upload PDFs/CSV for knowledge updates
🎨 Interactive UI with theme switching
🔗 Easy integration with college websites

---

## Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** FastAPI (Python)
- **Database:** Chroma vector database for semantic search
- **Version Control:** GitHub

---

## How it Works

1. **User sends a query** through the chat interface.
2. **Frontend JavaScript** captures the message and sends it to the backend API.
3. **FastAPI backend** processes the query:
   - Checks the vector database (Chroma) for semantic matches.
   - Searches uploaded PDFs/CSVs for relevant answers.
4. **Response is sent back** to the frontend in real-time.
5. **User sees the answer** in the chat window.

## Project Structure
CampusSarthi_ChatBot/ │ ├── 📂 frontend/ │ ├── index.html │ ├── static/ │ │ ├── style.css │ │ └── script.js │ └── Admin_UI/ │ ├── admin.html │ ├── admin.css │ ├── admin.js │ ├── login.html │ ├── login.css │ └── login.js │ ├── 📂 backend/ │ ├── main.py │ ├── faqs.json │ └── test_lang.py │ ├── 📂 vector_db/ # Stored embeddings (ChromaDB) ├── 📂 uploads/ # Uploaded PDFs/CSV files │ ├── .gitignore ├── README.md └── requirements.txt

## Installation

1.Clone the repository:

git clone https://github.com/Asmita-Rathod/CampusSarthi_ChatBot.git

cd CampusSarthi-chatbot

2.Create a virtual environment and activate it:

python -m venv venv
# Linux/Mac
source venv/bin/activate
# Windows
venv\Scripts\activate

3.Install dependencies:

pip install -r requirements.txt

4.Run the backend:

uvicorn backend.main:app --reload

5.Open the frontend:

Open frontend/index.html in a web browser.

## Usage

Chat with Campus Sarthi through the web interface.

Admins can upload PDFs/CSVs to update the chatbot knowledge base.

Switch languages using the language selector in the chat interface.
