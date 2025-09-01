# Gemini RAG AI Agent

An end-to-end Retrieval-Augmented Generation (RAG) pipeline built with **n8n**, **Google Gemini**, and **Supabase**.  
The agent retrieves information from documents (PDF/CSV) and provides contextual answers in real time.

---

## 📌 Features
- PDF/CSV knowledge base integration (Google Drive / local files)  
- Vector storage with **Supabase**  
- **Google Gemini** for embeddings + responses  
- Orchestrated via **n8n** workflow  
- Simple memory to manage chat sessions  
- End-to-end deployable pipeline  

---


---

## 📊 Workflow Diagram
<img width="1669" height="716" alt="Screenshot 2025-09-02 020929" src="https://github.com/user-attachments/assets/d5f1e7eb-fb46-4cf2-8d91-201ee1b2f867" />

---

## 🗂 Data Folder
These folder contains **sample documents** used as input for the RAG pipeline:  

- `sample knowledge base.docs` → Example knowledge base (docs from Google Drive)  

📌 These are **demo input files only**. Replace them with your own data when using the workflow.

---

## 🚀 Setup Instructions

### 1. Prerequisites
- [n8n](https://n8n.io) (self-hosted or cloud)  
- [Supabase](https://supabase.com) project (with pgvector enabled)  
- [Google Gemini API key](https://ai.google.dev)  

### 2. Configure the Pipeline in n8n
- Open n8n editor
- Create nodes for:
  - File ingestion (PDF/CSV)
  - Supabase vector storage
  - Google Gemini embeddings and response generation
  - chat interface triggers
- Update credentials:
  - **Supabase** → Project URL + API Key  
  - **Google Gemini** → API Key
- Connect the nodes according to the workflow steps above

### 3. Add Your Knowledge Base
- Upload PDFs or CSVs into gdrive
- Update n8n workflow to point to these docs  
- Run the pipeline → Embeddings are stored in Supabase  

### 4. Run a Chat
- Start conversation in n8n trigger  
- Query is vector-matched in Supabase  
- Google Gemini generates a contextual response  

---

## 📷 Demo Screenshots
### Workflow Execution
<img width="1667" height="708" alt="Screenshot 2025-09-02 014430" src="https://github.com/user-attachments/assets/3f2b8ab0-b371-4ccf-be80-7222cab83f33" />

### Chat Interface
<img width="1670" height="834" alt="Screenshot 2025-09-02 014601" src="https://github.com/user-attachments/assets/d933cc4e-f0c2-4f62-a28f-f08c7fb7962d" />

---

## 📊 Use Cases
- Document Q&A assistant
- Automated knowledge base chatbot
- Smart research assistant
- Data-driven insights from Google Drive
