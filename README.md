⚽ ProFaceScout AI  
Identify Famous Footballers from Images Using AI-Powered Facial Recognition + Groq's LLMs

📖 Overview

ProFaceScout is a smart web-based application that can identify famous football (soccer) players from uploaded images using facial recognition and Groq’s LLaMA-4-powered multimodal capabilities. The system detects faces, extracts the largest one, and queries Groq's API to return structured details like name, nationality, club, position, and major achievements.

Whether you’re a sports fan, analyst, or just exploring multimodal AI — this app is a fun and insightful demo of how computer vision + large language models can work together in real-time.

🚀 Features

- 🖼️ Upload an image with a football player’s face
- 🤖 Detect the player using Haar Cascade face detection + Groq’s LLaMA-4 model
- 📋 Get structured player info:
  - Full Name
  - Nationality
  - Current Club
  - Playing Position
  - Achievements (2–3 major titles)
- 🖼️ Output image with player name overlay and bounding box
- 🌐 Clean and interactive web UI via Flask

🧠 How It Works

1. 🧾 User uploads an image through the web interface.
2. 🎯 The app uses OpenCV's Haar Cascade to locate the largest face.
3. 🧠 The image is base64-encoded and sent to **Groq’s LLaMA-4 (Maverick 17B)** via their API.
4. 📊 Groq returns structured player details, which are displayed and also overlaid on the image.
5. 📁 Resulting image is saved and shown to the user.

![Screenshot 2025-06-16 205715](https://github.com/user-attachments/assets/0c442463-afbd-49c2-966e-fc01b07d82e4)
![output_detected](https://github.com/user-attachments/assets/bd7067cd-ee3e-4a1b-9e95-6d809d9a7a50)
![Screenshot 2025-06-16 205702](https://github.com/user-attachments/assets/f1587f14-f938-4668-812a-85d82e18708d)

🛠️ Tech Stack

- Python 3.x  
- OpenCV (face detection + image processing)  
- Flask (web application)  
- Groq API (multimodal LLM)  
- HTML/Jinja2 for front-end UI  

📂 Project Structure

profacescout/
├── app.py # Flask web app
├── main.py # CLI-based test interface
├── templates/
│ └── index.html # Web interface layout
├── static/uploads/ # Stores uploaded & result images
├── requirements.txt # Dependencies
└── README.md

🎯 Why It’s Useful
⚽ Combines real-time computer vision + LLM understanding

📷 Great for demos of multimodal reasoning

🧪 Can be extended to support other sports or celebrities

🎓 Perfect for AI students learning CV + LLMs + API integration

📄 License
MIT License — free to use, modify, and distribute with credit.

Built with 💡 Groq + OpenCV | Bringing AI recognition to the football field.
