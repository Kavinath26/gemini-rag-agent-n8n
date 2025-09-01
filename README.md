# 🚀 RAG AI Agent with n8n  

This project implements a **Retrieval-Augmented Generation (RAG) AI Agent** using **n8n**, **Google Gemini**, and **Supabase Vector Store**.  
It automates file ingestion from Google Drive, generates embeddings, stores them in Supabase, and powers a conversational AI agent with context-aware responses.  

---

## 📌 Features  

- ⚡ **Workflow Automation with n8n**  
  - File ingestion, embedding creation, and storage handled automatically.  

- 🤖 **AI Agent with Memory**  
  - Uses **Google Gemini Chat Model** with conversational memory.  

- 🔍 **RAG (Retrieval-Augmented Generation)**  
  - Retrieves embeddings from Supabase for context-aware responses.  

- 📂 **Google Drive Integration**  
  - Triggers when files are uploaded.  
  - Supports `.txt` and `.csv` extraction.  

- 🧠 **Embeddings**  
  - High-quality semantic embeddings generated via **Google Gemini**.  

---

## 🛠️ Tech Stack  

- **Workflow Orchestrator**: [n8n](https://n8n.io/)  
- **LLM**: Google Gemini  
- **Vector DB**: Supabase Vector Store  
- **Storage & Trigger**: Google Drive  
- **Embeddings**: Google Gemini  

---

## 📂 Workflow Overview  

1. **Google Drive Trigger** – Detects file uploads.  
2. **File Processing** – Extracts content (text or CSV).  
3. **Embeddings Generation** – Google Gemini creates embeddings.  
4. **Vector Store** – Stores embeddings in Supabase.  
5. **AI Agent** – Chat agent retrieves relevant context and responds.  

---

## 📸 Workflow Diagram  

![RAG AI Agent Workflow](workflows/rag_workflow.png)  

---



📊 Use Cases

Document Q&A assistant

Automated knowledge base chatbot

Smart research assistant

Data-driven insights from Google Drive
