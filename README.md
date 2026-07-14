
<div align="center">

###  *An Interactive AI-Powered Stock Market Investing Tutor for Beginners* 🤖

> Learn the fundamentals of stock market investing through interactive AI-powered conversations. 📈🤖

Built using **Python**, **Streamlit**, **Google Gemini API**, **Google Colab**, **ngrok**, and **GitHub** to provide an intelligent learning experience through a clean and responsive web interface.

<p align="center">
</p>


<br>

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge\&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-Web%20App-red?style=for-the-badge\&logo=streamlit)
![Google Gemini](https://img.shields.io/badge/Powered%20By-Gemini-4285F4?style=for-the-badge)
![Ngrok](https://img.shields.io/badge/Ngrok-Live%20Tunnel-black?style=for-the-badge)
![Google Colab](https://img.shields.io/badge/Google-Colab-F9AB00?style=for-the-badge\&logo=googlecolab)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)

</div>

---

##  Overview 📖

**AI Learning Buddy Srija** is an AI-powered educational assistant designed to make **Stock Market Investing** easy to understand for beginners.

The application serves as the user-facing **Streamlit** interface, while **Srija AI** acts as the internal AI engine responsible for prompt engineering, educational guardrails, and response orchestration using the **Google Gemini API**.

It helps learners understand investing concepts through simple explanations, real-life examples, interactive quizzes, and personalized question-answering, making financial education more engaging and accessible for beginners.

Built with **Python**, **Streamlit**, and the **Google Gemini API**, the application combines an intuitive web interface with carefully designed prompts to deliver beginner-friendly, interactive, and educational learning experiences.


The project can be executed using:

- 💻 Streamlit (Local)
- ☁️ Google Colab
- 🌍 Secure ngrok Tunnel

---

## 📸 Preview

| Explain Concept Page | Real- Life Learning Mode |
|-----------|---------------|
<img width="661" height="778" alt="Image" src="https://github.com/user-attachments/assets/206fca17-39f8-4059-9aab-9e00bc9290f8" />

<img width="666" height="716" alt="Image" src="https://github.com/user-attachments/assets/920cc0be-9901-4538-a5d0-5ff5d6c30551" />
</p>

| Quiz | Ask Anything |
|------|--------------|
<img width="741" height="826" alt="Image" src="https://github.com/user-attachments/assets/1ff8152d-b2b8-4520-ad73-c924c7a0a9d8" />

<img width="655" height="769" alt="Image" src="https://github.com/user-attachments/assets/86d4c9e8-df72-41f2-8099-45a7737f5b16" />
</p>

---

## System Architecture 🏗️

```mermaid
flowchart LR

Student["👩‍🎓 Student"]

Browser["🌐 Browser"]

Frontend["🎓 AI Learning Buddy Srija
(Streamlit Frontend)"]

Tunnel["🌍 Secure Ngrok Tunnel"]

Backend["🧠 Srija AI
(Core Engine)"]

Gemini["🤖 Gemini API"]

Student --> Browser
Browser --> Frontend
Frontend --> Tunnel
Tunnel --> Backend
Backend --> Gemini
Gemini --> Backend
Backend --> Tunnel
Tunnel --> Frontend
Frontend --> Student
```

---

##  Naming Architecture 🏷️

To maintain a clean separation between the presentation layer and backend logic, two different system names are intentionally used.

| Layer       | Name                        | Purpose                                                |
| ----------- | --------------------------- | ------------------------------------------------------ |
| 🎨 Frontend       | AI Learning Buddy Srija | User-facing Streamlit application                                                             |
| 🧠 AI Logic Layer | Srija AI                | Prompt engineering, educational guardrails, tutoring logic, and response orchestration |
| 🤖 AI Model       | Google Gemini API       | Generates AI-powered responses                                                         |


---

##  Complete Application Workflow 🔄

```mermaid
flowchart TD

A([🚀 Start])

B["🌐 Student Opens Application"]

C["⌨️ Student Types a Question"]

D["🖥️ Streamlit Captures Prompt"]

E["🔐 Load Environment Variables"]

F["🌍 Route Request Through Ngrok"]

G["🧠 Srija AI Processes Prompt"]

H["🤖 Gemini API Generates Response"]

I["📚 Educational Response Returned"]

J["✨ Streamlit Displays Answer"]

K([✅ Ready for Next Question])

A --> B
B --> C
C --> D
D --> E
E --> F
F --> G
G --> H
H --> I
I --> J
J --> K
```

---

##  Request Lifecycle ⚡

```mermaid
sequenceDiagram

participant Student
participant Streamlit
participant Ngrok
participant SrijaAI
participant Gemini

Student->>Streamlit: Ask Question

Streamlit->>Ngrok: Send Prompt

Ngrok->>SrijaAI: Forward Request

SrijaAI->>Gemini: Generate Response

Gemini-->>SrijaAI: AI Answer

SrijaAI-->>Ngrok: Return Result

Ngrok-->>Streamlit: Stream Response

Streamlit-->>Student: Display Answer
```

---

##  Component Architecture 🧩

```mermaid
graph TD

subgraph USER
A[👩‍🎓 Student]
end

subgraph FRONTEND
B[🎓 AI Learning Buddy Srija]
end

subgraph NETWORK
C[🌐 Ngrok Tunnel]
end

subgraph BACKEND
D[🧠 Srija AI]
E[📝 Prompt Engineering]
F[🛡 Educational Guardrails]
end

subgraph AI
G[🤖 Gemini API]
end

A --> B
B --> C
C --> D
D --> E
E --> F
F --> G
G --> D
D --> B
```

---

##  Deployment Architecture ☁️

```mermaid
flowchart LR

Colab["☁️ Google Colab"]

Local["💻 Local Machine"]

Streamlit["🎓 Streamlit App"]

Ngrok["🌍 Secure Ngrok Tunnel"]

Browser["🌐 Student Browser"]

Gemini["🤖 Gemini API"]

Colab --> Streamlit
Local --> Streamlit

Streamlit --> Ngrok

Ngrok --> Browser

Streamlit --> Gemini
```

---

---

## 📂 Project Structure

```text
AI-Learning-Buddy-Srija/
│
├── app.py                      # Main Streamlit application
├── requirements.txt            # Project dependencies
├── README.md                   # Project documentation
├── .gitignore                  # Git ignore rules
├── .env.example                # Environment variable template
│
├── notebooks/
│   └── AI_Learning_Buddy.ipynb # Google Colab notebook
│
└── assets/
    ├── banner.png              # Project banner
    └── screenshots/            # Application screenshots
```

---

## ✨ Key Features

- 📈 Beginner-friendly AI tutor for **Stock Market Investing**
- 🤖 AI-powered explanations using **Google Gemini 2.5 Flash**
- 🌍 Real-life examples to simplify complex investing concepts
- 📝 Automatic 5-question MCQ quiz generation with answers
- 💬 "Ask Anything" mode for personalized learning
- ⚡ Instant AI-generated responses
- 🌐 Public deployment using **ngrok**
- 🔐 Secure API key management with environment variables
- ☁️ Compatible with **Google Colab** and local execution
- 📱 Clean, responsive, and user-friendly Streamlit interface

---

## 📚 Learning Modes

Students can choose from four different learning modes depending on how they want to learn.

| Learning Mode | Description |
| :--- | :--- |
| 📖 Explain Concept | Explains stock market concepts in simple, beginner-friendly language. |
| 🌍 Real-Life Example | Uses everyday examples and analogies to improve understanding. |
| 📝 Generate Quiz | Creates five multiple-choice questions with correct answers. |
| 💬 Ask Anything | Allows learners to ask any stock market or investing-related question. |

---

## 🛠️ Technology Stack

| Technology | Purpose |
| :--- | :--- |
| Python | Core application development |
| Streamlit | Interactive web interface |
| Google Gemini API | AI-powered response generation |
| Google Colab | Cloud-based development environment |
| ngrok | Public deployment and secure tunneling |
| python-dotenv | Secure environment variable management |
| GitHub | Version control and project hosting |

---

## 🚀 Running the Project

## ☁️ Option 1 — Google Colab (Recommended)

1. Open the notebook in **Google Colab**.
2. Add your **Google Gemini API Key**.
3. Add your **ngrok Authentication Token**.
4. Run all notebook cells.
5. The notebook will:
   - Launch the Streamlit application
   - Create a secure ngrok tunnel
   - Generate a public URL
6. Open the generated URL in your browser.

---

## 💻 Option 2 — Run Locally

### Step 1 — Create a `.env` file

```env
GEMINI_API_KEY=YOUR_API_KEY
NGROK_AUTH_TOKEN=YOUR_NGROK_TOKEN
```

### Step 2 — Install dependencies

```bash
pip install -r requirements.txt
```

### Step 3 — Launch the application

```bash
streamlit run app.py
```
## 🌐 Live Demo

🚀 **Try the application here:**

https://ai-learning-buddy-srija.streamlit.app/

## 📌 Execution Pipeline

```mermaid
flowchart LR

Question["❓ Student Question"]

Prompt["📝 Prompt Processing"]

AI["🧠 Srija AI"]

Gemini["🤖 Google Gemini API"]

Response["📚 Educational Response"]

Display["✨ Streamlit Interface"]

Question --> Prompt
Prompt --> AI
AI --> Gemini
Gemini --> Response
Response --> Display
```

---

## 📊 System Flow Summary

```text
Student
   │
   ▼
AI Learning Buddy Srija
(Streamlit)

   │
   ▼
ngrok Tunnel

   │
   ▼
Prompt Processing

   │
   ▼
Google Gemini API

   │
   ▼
AI Response

   │
   ▼
Student Interface
```

---

## 👩‍💻 Project Information

| Field | Details |
| :--- | :--- |
| Developer | **Srija Bhattacharya** |
| Project | **AI Learning Buddy Srija** |
| Domain | **Stock Market Investing** |
| AI Model | **Google Gemini 2.5 Flash** |
| Program | **AI Empower(H)er Program** |

---

## 💡 Future Enhancements

- 📊 Interactive stock market charts
- 🎤 Voice-enabled AI tutoring
- 🌐 Multi-language support
- 📈 Personalized learning recommendations
- 📝 Adaptive quizzes based on learner performance
- 📄 Export notes and quizzes as PDF
- 🏆 Student learning progress dashboard

---
---

## ❤️ Acknowledgements


This project was developed as part of the **AI Empower(H)er Program**.

Special thanks to:

- 💙 Dr. Pallavi Khanna Ma'am
- 💙 Infosys Springboard
- 💙 Skillsoft

for creating a platform where learners from every background can explore Generative AI, build real-world projects, and gain hands-on experience through the AI Empower(H)er Program.

## ⭐ Support

If you enjoyed exploring this project or found it useful, consider giving it a ⭐ on GitHub. 
It helps support the project and encourages future improvements.


## 📄 License

This project is intended for educational purposes as part of the AI Empower(H)er Program.


<p align="center">
Made with ❤️ by <b>Srija Bhattacharya</b>
</p>

</div>
