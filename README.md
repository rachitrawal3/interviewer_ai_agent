
---

# 🤖 Excel Data Analyst Mock Interview Bot

An **AI-powered prototype system** for automating mock interviews for the **Excel Data Analyst role**.
Built using **Microsoft AutoGen**, **Groq API**, and **Streamlit**, it simulates an interactive interview flow, generates customizable questions, records candidate responses, and produces automated evaluation reports.

---

## 💡 Features

* 📝 **Dynamic Question Generator**
  Generates unique interview questions in JSON format based on a flexible system prompt.
  ➔ Customize number, type (theoretical, practical, scenario-based), and topics (e.g., PivotTables, data cleaning).

* 💬 **Interactive Interview Flow**
  Sequentially asks questions and records typed responses in a simple web-based chat interface powered by Streamlit.

* ✅ **Automated Evaluation Report**
  Analyzes the full transcript and generates a structured report with:

  * Candidate strengths
  * Weaknesses
  * Clear "HIRE" or "NO HIRE" recommendation

* ⚡️ **Fully Configurable Design**
  Modify the system prompt to easily change:

  * Number of questions
  * Type of questions
  * Focused Excel topics
    No code changes required.

* 🗂️ **In-Memory State Management**
  Uses `InMemoryDB` and Streamlit’s `session_state` to manage session messages and interview progress.

* ⚠️ **Prototype Implementation**
  Designed for experimentation and demos:

  * No FastAPI backend
  * No persistent database
  * All state is stored in-memory

---

## 🧱 Tech Stack

| Technology            | Purpose                                            |
| --------------------- | -------------------------------------------------- |
| **Python & Asyncio**  | Async handling of agent interactions               |
| **Microsoft AutoGen** | Agent orchestration and system design              |
| **Groq API**          | LLM backend for question generation and evaluation |
| **Streamlit**         | Interactive web interface                          |
| **InMemoryDB**        | Temporary storage of session state and messages    |

---

## ⚙️ How It Works

1. ✅ **Question Generation**
   The system generates a set of configurable interview questions via a custom system prompt.

2. 💬 **Interview Process**

   * The Interviewer Agent asks one question at a time.
   * The User Proxy Agent records the candidate’s answer.
   * The process repeats until all questions are answered.

3. 📄 **Automated Evaluation**
   The full transcript is sent to the Evaluation Agent, which returns a structured report.

---

## ⚠️ Prototype Notice

This is a **proof-of-concept prototype**:

* No backend (FastAPI)
* No persistent storage (only in-memory)
* Focused on demonstrating agent orchestration and AI-driven interview flow.

➡️ Perfect for demos, prototyping, and experimentation.

---

## 🚀 Next Steps

For production readiness:

* Add FastAPI backend
* Implement a persistent database (e.g., PostgreSQL)
* Add authentication & session management
* Expand to support multiple interview roles

---

⚡️ Simple, flexible, and intelligent mock interview automation built to demonstrate the power of AI agents.

---

<p align="center">
  <img src="https://user-images.githubusercontent.com/your-username/architecture-diagram.png" alt="Architecture Diagram" width="60%">
</p>

---

