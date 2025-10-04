# MedBot – AI-Powered Healthcare Chatbot

## 📌 Overview
MedBot is an AI-powered healthcare chatbot that allows users to ask medical-related questions and get AI-generated answers in a conversational manner.  
It uses **LangChain**, **GPT models**, and **Pinecone vector database** to provide context-aware responses based on a medical knowledge base.  
The project is built with **Flask** for the backend, includes a simple web-based frontend, and is fully containerized with **Docker** for deployment.

---

## 🚀 Features
- 💬 **Conversational Chatbot** – Ask medical-related queries and get quick responses.  
- 📖 **Knowledge Base** – Uses a medical book (PDF) converted into embeddings for accurate retrieval.  
- 🧠 **Generative AI** – Powered by OpenAI GPT integrated with LangChain.  
- 🔎 **Vector Search** – Pinecone is used to store and retrieve embeddings.  
- 🌐 **Web Interface** – User-friendly chat UI built with Flask, HTML, and CSS.  
- 🐳 **Containerized** – Packaged using Docker for easy deployment.  
- ☁️ **Cloud Ready** – Deployment supported on AWS with CI/CD (GitHub Actions).  

---

## 🛠 Tech Stack
- **Backend:** Python, Flask, LangChain, OpenAI GPT  
- **Database:** Pinecone (Vector Database for embeddings)  
- **Frontend:** HTML, CSS (chat interface)  
- **Deployment:** Docker, AWS, GitHub Actions  
- **Other Tools:** HuggingFace (embeddings), dotenv (env management)  

---

## 📂 Project Structure
├── app.py # Main Flask application
├── store_index.py # Creates Pinecone index from medical PDF
├── src/
│ ├── helper.py # Utility functions (load PDF, split text, embeddings)
│ ├── prompt.py # Prompt template for GPT responses
├── templates/
│ └── chat.html # Chatbot frontend
├── static/
│ └── style.css # Styling for chatbot UI
├── Data/
│ └── Medical_book.pdf # Knowledge base
├── Dockerfile # Docker container setup
├── requirements.txt # Project dependencies
└── README.md # Project documentation
