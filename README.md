# 🌐 Web Browsing Multi-Agent Automation System

A local **multi-agent browser automation system** built using CrewAI and Stagehand that can perform web tasks from natural language queries.

This project demonstrates how autonomous AI agents can collaboratively plan, execute, and summarize browser-based tasks—just like a human using the web.

---

## 🚀 Features

* 🤖 Multi-agent architecture using CrewAI
* 🌐 AI-powered browser automation with Stagehand
* 🧠 Natural language → structured task execution
* 📊 Clean and user-friendly output generation
* 💻 Runs locally using Ollama (no API cost)

---

## 🧠 How It Works

1. **Query Submission**
   User provides a natural language query (e.g., *“Find the latest iPhone price on Amazon”*)

2. **Task Planning (Planner Agent)**
   Converts the query into a structured automation plan (URL + steps)

3. **Execution (Browser Agent)**
   Uses Stagehand + Playwright to:

   * Open websites
   * Interact with elements
   * Extract data

4. **Response Synthesis (Synthesis Agent)**
   Formats raw data into a clean, readable response

5. **Final Output**
   Returns a polished result to the user

---

## 🛠️ Tech Stack

* **CrewAI** – Multi-agent orchestration
* **Stagehand** – AI browser automation
* **Playwright** – Browser control
* **Ollama** – Local LLM runtime
* **Python** – Core backend

---

## ⚙️ Setup Instructions

Follow these steps to run the project locally:

---

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

---

### 2️⃣ Create Environment File

Create a `.env` file in the root directory:

```env
OPENAI_API_KEY=dummy
MODEL_API_KEY=dummy
```

> If using Ollama locally, no real API key is required.

---

### 3️⃣ Install Ollama

Download from: https://ollama.com/download

Then pull the required model:

```bash
ollama pull gpt-oss
```

---

### 4️⃣ Install Dependencies

```bash
pip install uv
uv sync
```

Activate virtual environment:

```bash
source .venv/bin/activate
# Windows:
.venv\Scripts\activate
```

---

### 5️⃣ Install Playwright Browsers

```bash
playwright install
```

---

### ▶️ Run the Project

```bash
python flow.py
```

---

## 📌 Example Use Cases

* 🔍 Product price extraction (Amazon, Flipkart)
* 💼 Job listings automation
* 📊 Data scraping from websites
* 🔎 Research automation

---


---

## 🤝 Contribution

Contributions are welcome!
Feel free to fork the repo and submit a pull request.
