
<div align="center">

###  *An Interactive AI-Powered Stock Market Investing Tutor for Beginners* 🤖

Built using **Python**, **Streamlit**, **Google Gemini API**, **Google Colab**, **ngrok**, and **GitHub** to provide an intelligent learning experience through a clean and responsive web interface.
<br>

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge\&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-Web%20App-red?style=for-the-badge\&logo=streamlit)
![Gemini](https://img.shields.io/badge/Powered%20By-Gemini-4285F4?style=for-the-badge)
![Ngrok](https://img.shields.io/badge/Ngrok-Live%20Tunnel-black?style=for-the-badge)
![Google Colab](https://img.shields.io/badge/Google-Colab-F9AB00?style=for-the-badge\&logo=googlecolab)

</div>

---

##  Overview 📖

**AI Learning Buddy Srija** is an AI-powered educational assistant designed to make **Stock Market Investing** easy to understand for beginners.

The application explains investing concepts in simple language, provides real-life examples, generates quizzes, and answers students' questions interactively.

Built using **Streamlit** and powered by the **Google Gemini API**, the application uses carefully designed prompts to produce beginner-friendly, engaging, and educational responses.

The project can be executed using:

- 💻 Streamlit (Local)
- ☁️ Google Colab
- 🌍 Secure ngrok Tunnel

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
| 🎨 Frontend | **AI Learning Buddy Srija** | Interactive Streamlit application for learners |
| ⚙ AI Engine | **Google Gemini API**         | Generates educational responses |
| 🧠 Prompt Layer | **Custom Prompt Engineering** | Ensures beginner-friendly and structured explanations |

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

##  Project Structure 📂

AI-Learning-Buddy-Srija
│
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
├── .env.example
│
├── notebooks/
│   └── AI_Learning_Buddy.ipynb
│
└── assets/
    ├── banner.png
    └── screenshots/
```

---

##  Key Features ✨

- 📈 Beginner-friendly Stock Market Investing tutor
- 🤖 AI-powered explanations using Google Gemini
- 🌍 Real-life examples and easy-to-understand analogies
- 📝 Automatic MCQ quiz generation
- 💬 Ask Anything mode for personalized learning
- ⚡ Real-time AI responses
- 🌐 Secure deployment using ngrok
- 🔐 Secure API key management
- ☁️ Google Colab compatible
- 💻 Local execution support
- 📱 Clean and responsive Streamlit interface

---

##  Learning Modes 📚

Students can choose from four different learning modes.

| Mode | Description |
|------|-------------|
| 📖 Explain Concept | Explains stock market concepts in beginner-friendly language |
| 🌍 Real-Life Example | Connects concepts with practical everyday examples |
| 📝 Generate Quiz | Creates multiple-choice quizzes with answers |
| 💬 Ask Anything | Allows students to ask any investing-related question |

---

##  Technology Stack 🛠️

| Technology    | Purpose                      |
| ------------- | ---------------------------- |
| Python         | Core application development |
| Streamlit      | Interactive web interface |
| Google Gemini API | AI response generation |
| Google Colab | Cloud development |
| ngrok | Public deployment |
| python-dotenv | Secure environment variables |
| GitHub | Version control |

---

##  Running the Project  🚀

##  Option 1 — Google Colab (Recommended) ☁️

1. Open the provided notebook in Google Colab.
2. Add your Gemini API Key.
3. Add your Ngrok Authentication Token.
4. Run all notebook cells.
5. The notebook automatically:

   * launches the Streamlit application
   * creates a secure Ngrok tunnel
   * generates a public URL
6. Open the generated URL in your browser.

---

###  Option 2 — Run Locally 💻

### Step 1

Create a `.env` file

```GEMINI_API_KEY=YOUR_API_KEY
NGROK_AUTH_TOKEN=YOUR_NGROK_TOKEN
```

---

### Step 2

Install dependencies

```bash
pip install -r requirements.txt
```

---

### Step 3

Run the application

```bash
streamlit run app.py
```

---

##  Execution Pipeline 📌

```mermaid
flowchart LR

Question["❓ Student Question"]

Prompt["📝 Prompt Processing"]

AI["🧠 Srija AI"]

Gemini["🤖 Gemini"]

Response["📚 Educational Response"]

Display["✨ Streamlit Interface"]

Question --> Prompt
Prompt --> AI
AI --> Gemini
Gemini --> Response
Response --> Display
```

---

##  System Flow Summary 📊

```text
Student
   │
   ▼
AI Learning Buddy Srija
(Streamlit)

   │

   ▼
Ngrok Tunnel

   │

   ▼
Srija AI Core

   │

   ▼
Gemini API

   │

   ▼
Educational Response

   │

   ▼
Student Interface
```

---

##  Project Information 👩‍💻

| Field          | Details                     |
| -------------- | --------------------------- |
| Developer | **Srija Bhattacharya** |
| Project | **AI Learning Buddy Srija** |
| Domain | **Stock Market Investing** |
| AI Model | **Google Gemini 2.5 Flash** |
| Program | **AI EMPOWER(H)ER Program** |
---

##  Future Enhancements 💡

- 📊 Interactive stock charts
- 🎤 Voice-enabled tutoring
- 🌍 Multi-language support
- 📝 Adaptive quizzes based on learner performance
- 📈 Personalized learning roadmap
- 📄 Export notes and quizzes as PDF
- 🏆 Student progress dashboard

---

#  Acknowledgements ❤️

This project was developed as part of the **AI EMPOWER(H)ER Program**.

A heartfelt thank you to:

- 💙 Dr. Pallavi Khanna
- 💙 Infosys Springboard
- 💙 Skillsoft

for creating an inspiring platform where learners from all backgrounds can explore Generative AI, build real-world projects, and grow through hands-on learning.

---

<div align="center">

##  Support ⭐

If you found this project useful or interesting, consider giving it a ⭐ on GitHub!


**Made with ❤️ by Srija Bhattacharya**

</div>
