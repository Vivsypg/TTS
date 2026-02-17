
Frog Story Text-to-Speech API Project

Student: Mahesh
Class: 8

Description:
This project converts story text into speech audio using Python Text-to-Speech.
It exposes an API that can be integrated into websites (Node/Next.js).

Technology:
- Python
- Flask API
- pyttsx3 speech engine
- Next.js frontend integration

How to run:

1. Install Python
2. Install requirements:
   pip install -r requirements.txt
3. Run API:
   python tts_api.py
4. Open browser:
   http://127.0.0.1:5000

API usage:
POST /tts
Body:
{ "text": "Hello" }

Returns:
Speech audio file
