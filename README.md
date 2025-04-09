# Chatbot
![image](https://github.com/Kabhishek021/Q-A-chatbot/blob/main/chatbot.png)
Here's a clean and professional `README.md` document for your LangChain + Ollama + Streamlit demo project:

---

# 🚀 LangChain + Ollama + Streamlit Demo

This project is a simple demonstration of how to integrate **LangChain**, **Ollama**, and **Streamlit** to build an interactive LLM-based Q&A assistant. The application takes a user's question from a Streamlit UI, passes it through a LangChain prompt pipeline, and responds using the **Ollama Gemma 2B** model.

---

## 📂 Project Structure

```
├── app.py                  # Streamlit application code
├── .env                   # Environment variables (API keys etc.)
└── README.md              # Project documentation
```

---

## 🔧 Requirements

Install the following Python packages:

```bash
pip install streamlit langchain langchain-core langchain-community python-dotenv
```

Also ensure **Ollama** is installed and running on your system with the required model.

Install Ollama:  
👉 https://ollama.com/download

Pull the model:

```bash
ollama pull gemma:2b
```

---

## 🔑 Environment Variables

Create a `.env` file in your project root and add the following:

```env
LANGCHAIN_API_KEY=your_langchain_api_key_here
```

> **Note**: If you don’t have a LangChain API key, you can remove the tracking functionality by commenting out that section.

---

## ▶️ How to Run

```bash
streamlit run app.py
```

---

## 💡 Features

- Simple **Q&A chatbot UI**
- Uses **LangChain prompt templates**
- **Ollama LLM (Gemma 2B)** as the backend model
- Output parsing using **StrOutputParser**
- Clean and minimal **Streamlit interface**

---

## 🧠 How It Works

1. User enters a question in the input box.
2. The question is passed through a **LangChain prompt template**.
3. The prompt is processed by **Ollama (Gemma 2B)** model.
4. The model response is parsed and displayed using **Streamlit**.

---

## 📝 Sample Prompt Template

```python
prompt = ChatPromptTemplate.from_messages(
    [
        ('system', 'You are a helpful assistant. Please respond to the user question.'),
        ('user', "Question: {question}")
    ]
)
```

---

## 📸 Screenshot (optional)
You can add a screenshot here to visualize the UI.

---




