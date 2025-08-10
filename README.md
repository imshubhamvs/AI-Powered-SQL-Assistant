# 🧠 AI-Powered SQL Assistant

An **AI-powered natural language to SQL assistant** that allows users to query databases using plain English.  
It converts user queries into **optimized SQL statements**, executes them, and returns results — without requiring SQL knowledge.

---

## 📌 Table of Contents
- [About the Project](#-about-the-project)
- [Tech Stack](#-tech-stack)
- [Machine Learning Process](#-machine-learning-process)
- [Project Demo](#-project-demo)
- [How to Run Locally](#-how-to-run-locally)
- [Future Improvements](#-future-improvements)
- [License](#-license)

---

## 📖 About the Project

The **AI-Powered SQL Assistant** bridges the gap between non-technical users and complex database systems.  
Instead of writing SQL queries manually, users can simply type:

> "Show me the top 5 customers by total purchases last month."

The assistant:
1. Understands the intent using **Natural Language Processing (NLP)**.
2. Generates the appropriate SQL query.
3. Executes it on the target database.
4. Returns results in a clean, readable format.

---

## 🛠 Tech Stack

### **Frontend**
- **React.js** — Interactive chat-based UI
- **HTML/CSS** — Styling & layout
- **Axios** — API calls to backend

### **Backend**
- **Node.js + Express** — API handling & server logic
- **LangChain** — Prompt engineering & LLM orchestration
- **Groq API (Open-source LLM)** — SQL query generation
- **Vector Database** — Context storage & retrieval (Pinecone / Chroma / Milvus)
- **MySQL / PostgreSQL** — Query execution on target DB

### **Others**
- **Socket.IO (Optional)** — Real-time responses
- **dotenv** — Environment variable handling

---

## 🤖 Machine Learning Process

The AI workflow follows these steps:

1. **User Input** — A natural language query is entered in the chat.
2. **Context Retrieval** — Vector database stores and retrieves relevant past conversations.
3. **Prompt Engineering** — LangChain formats the prompt with schema & context.
4. **SQL Generation** — Groq LLM generates SQL query.
5. **Query Validation** — Sanitizer ensures no harmful queries (`DROP`, `DELETE` without conditions, etc.).
6. **Database Execution** — Runs query on target DB.
7. **Result Formatting** — Sends clean table format back to frontend.

User → Backend → LangChain → LLM → SQL Query → DB → Results → User


---

## 📷 Project Demo

### **Execution Screenshots**

| ![User Query](path/to/query_scr![WhatsApp Image 2025-08-11 at 00 52 24_46b3d9da](https://github.com/user-attachments/assets/f23891b5-1ce7-4b2e-9946-dba0fab3501d)
eenshot.png) |![WhatsApp Image 2025-08-11 at 00 50 18_3f77d3d2](https://github.com/user-attachments/assets/4921389b-5d98-4cd9-889c-05128580007a)
 !![WhatsApp Image 2025-08-11 at 00 29 48_181f2ccc](https://github.com/user-attachments/assets/cd4f8d14-ece9-48cc-b289-29e3a9b23cac)


---

## 🚀 How to Run Locally

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/your-username/ai-sql-assistant.git
cd ai-sql-assistant

2️⃣ Install Dependencies
Backend:

bash
Copy
Edit
cd backend
npm install
Frontend:

bash
Copy
Edit
cd frontend
npm install
3️⃣ Set Environment Variables
Create a .env file in the backend directory:

PORT=5000
GROQ_API_KEY=your_groq_api_key
VECTOR_DB_URL=your_vector_db_url
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=your_database

4️⃣ Start the Backend
bash
Copy
Edit
cd backend
npm run dev
5️⃣ Start the Frontend
bash
Copy
Edit
cd frontend
npm start
🔮 Future Improvements

Fine-tuned model for domain-specific queries.

Export results to Excel/CSV.


---

If you want, I can now **add a professional architecture diagram** for this README so it looks visually appealing and explains your system flow at a glance.  

Do you want me to add that diagram now?


**Flow Diagram**:
