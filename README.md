 🏥 AI-Powered Insurance Claim Analyzer (RAG Based)

An intelligent Insurance Claim Analysis system built using **Retrieval-Augmented Generation (RAG)**.

This application analyzes insurance claims using real policy documents and generates structured decisions such as:

- ✅ Approved  
- ❌ Rejected  
- ⚠ Needs Review  

The system uses vector embeddings and a local LLM to ensure context-aware and policy-based reasoning.

---

## 🚀 Project Overview

Insurance policy documents are lengthy and complex. Manual claim verification is:

- Time-consuming
- Error-prone
- Legally intensive
- Dependent on expert knowledge

This project automates initial claim evaluation using AI while grounding responses strictly in policy clauses.

---

## 🧠 How It Works (RAG Pipeline)

1. Upload insurance policy document (PDF)
2. Extract and chunk policy text
3. Convert chunks into embeddings
4. Store embeddings in ChromaDB
5. User submits claim details
6. System retrieves relevant policy clauses
7. LLM analyzes claim using retrieved context
8. Structured JSON decision is generated
9. Email-ready formatted output is displayed

---

## 🏗️ System Architecture


User Uploads Policy
↓
PDF Text Extraction
↓
Chunking
↓
Embedding Model (nomic-embed-text)
↓
ChromaDB (Vector Storage)
↓
User Enters Claim + Date of Incident
↓
Retrieve Relevant Policy Clauses
↓
LLM (phi3 via Ollama)
↓
Structured JSON Output
↓
Email / Automation Integration


---

## 🛠 Technologies Used

- **Python**
- **Streamlit** – UI
- **ChromaDB** – Vector Database
- **Ollama** – Local LLM Hosting
- **nomic-embed-text** – Embedding Model
- **phi3-mini** – Language Model
- **PyPDF** – PDF Text Extraction

---

## 📅 Key Features

- 🔎 Retrieval-Augmented Generation (RAG)
- 📄 Real Policy Document Support
- 🧠 Context-Aware AI Decisions
- 📊 Structured JSON Output
- 📧 Email-Ready Claim Response
- 📆 Waiting Period Logic using Date of Incident
- 🔐 Fully Local (No API Cost)

---

## 📥 Input Fields

- Customer Name
- Policy ID
- Claim Amount
- Policy Start Date
- Date of Incident
- Claim Description

The system calculates:


Policy Active Days = Date of Incident - Policy Start Date


This enables automatic waiting-period evaluation.

---

