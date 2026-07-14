# 🎓 AI Learning Buddy Srija

<div align="center">

### 🤖 *An Interactive AI-Powered Learning Assistant for Students*

Built using **Python**, **Streamlit**, **Gemini API**, and **Ngrok** to provide an intelligent educational experience through a clean and responsive web interface.

<br>

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge\&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-Web%20App-red?style=for-the-badge\&logo=streamlit)
![Gemini](https://img.shields.io/badge/Powered%20By-Gemini-4285F4?style=for-the-badge)
![Ngrok](https://img.shields.io/badge/Ngrok-Live%20Tunnel-black?style=for-the-badge)
![Google Colab](https://img.shields.io/badge/Google-Colab-F9AB00?style=for-the-badge\&logo=googlecolab)

</div>

---

# 📖 Overview

**AI Learning Buddy Srija** is an AI-powered educational assistant designed to help students learn interactively through natural language conversations.

The application is built using **Streamlit** as the frontend interface while a dedicated backend workspace (**Srija AI**) manages prompt engineering, educational guardrails, and AI response generation.

The project can be executed either:

* 💻 Locally using Streamlit
* ☁️ Through Google Colab
* 🌍 Publicly via a secure Ngrok Tunnel

---

# 🏗️ System Architecture

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

# 🏷️ Naming Architecture

To maintain a clean separation between the presentation layer and backend logic, two different system names are intentionally used.

| Layer       | Name                        | Purpose                                                |
| ----------- | --------------------------- | ------------------------------------------------------ |
| 🎨 Frontend | **AI Learning Buddy Srija** | Student-facing Streamlit application                   |
| ⚙ Backend   | **Srija AI**                | Core AI workspace, prompt engineering and system logic |

---

# 🔄 Complete Application Workflow

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

# ⚡ Request Lifecycle

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

# 🧩 Component Architecture

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

# ☁️ Deployment Architecture

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

# 📂 Project Structure

```text
AI-Learning-Buddy-Srija
│
├── app.py
├── requirements.txt
├── README.md
├── .env
│
├── assets/
│   ├── banner.png
│   ├── architecture.png
│   └── workflow.png
│
└── notebooks/
    └── AI_Learning_Buddy.ipynb
```

---

# ✨ Key Features

* 🎓 Interactive AI-powered educational assistant
* 🤖 Customized prompt engineering for student learning
* ⚡ Real-time AI-generated responses
* 🌐 Secure public deployment using Ngrok
* 🖥 Clean and responsive Streamlit interface
* 🔐 Secure API key management using `.env`
* ☁️ Google Colab compatible
* 💻 Local execution support

---

# 🛠️ Technology Stack

| Technology    | Purpose                      |
| ------------- | ---------------------------- |
| Python        | Application Development      |
| Streamlit     | Frontend Web Interface       |
| Gemini API    | AI Response Generation       |
| Python Dotenv | Secure Environment Variables |
| Ngrok         | Public Tunnel                |
| Google Colab  | Cloud Development            |

---

# 🚀 Running the Project

## ☁️ Option 1 — Google Colab (Recommended)

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

## 💻 Option 2 — Run Locally

### Step 1

Create a `.env` file

```env
API_KEY=YOUR_API_KEY
```

---

### Step 2

Install dependencies

```bash
pip install streamlit python-dotenv pyngrok
```

---

### Step 3

Run the application

```bash
streamlit run app.py
```

---

# 📌 Execution Pipeline

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

# 📊 System Flow Summary

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

# 👩‍💻 Project Submission

| Item           | Details                     |
| -------------- | --------------------------- |
| Student Name   | **Srija Bhattacharya**      |
| Program        | **AI Empower(H)er Program** |
| Application    | **AI Learning Buddy Srija** |
| Backend Engine | **Srija AI**                |

---

# 💡 Future Enhancements

* 📄 PDF generation
* 🎤 Voice-based interaction
* 🌐 Multi-language support
* 📊 Learning progress analytics
* 📝 Personalized quizzes
* 📚 Learning history
* 🎓 Adaptive learning recommendations

---

# ❤️ Acknowledgements

Special thanks to:

* 💙 **Skillsoft**
* 💙 **Infosys Springboard**
* 💙 **AI Empower(H)er Program**
* 💙 **Dr. Pallavi Khanna**

for providing an incredible opportunity to explore Generative AI and build meaningful AI-powered educational solutions.

---

<div align="center">

## ⭐ If you found this project interesting, don't forget to star the repository!

**Made with ❤️ by Srija Bhattacharya**

</div>
