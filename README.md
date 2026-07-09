# 📄 Context-Aware RAG Chatbot

A **Context-Aware Retrieval-Augmented Generation (RAG) Chatbot** built using **LangChain**, **FAISS**, **Hugging Face Transformers**, and **Gradio**. The chatbot allows users to upload PDF documents and ask questions based on their content using semantic search and a Large Language Model (LLM).

---

## 🚀 Features

- 📄 Upload and process PDF documents
- ✂️ Split documents into semantic text chunks
- 🔍 Generate embeddings using Sentence Transformers
- 🗂️ Store embeddings in a FAISS vector database
- 🤖 Answer questions using Retrieval-Augmented Generation (RAG)
- 💬 Interactive chatbot interface with Gradio
- 💾 Save and reload FAISS vector index
- 🆓 Uses free Hugging Face models (No OpenAI API required)

---

## 🛠️ Technologies Used

- Python
- Google Colab
- LangChain
- Hugging Face Transformers
- Sentence Transformers
- FAISS
- PyPDF
- Gradio

---

## 📂 Project Structure

```
Context_Aware_RAG_Chatbot/
│
├── Context_Aware_RAG_Chatbot.ipynb
├── README.md
├── requirements.txt
├── faiss_index/
│   ├── index.faiss
│   └── index.pkl
├── sample.pdf
└── screenshots/
```

---

## ⚙️ Installation

Install the required libraries:

```bash
pip install langchain
pip install langchain-community
pip install langchain-huggingface
pip install langchain-text-splitters
pip install sentence-transformers
pip install transformers
pip install faiss-cpu
pip install pypdf
pip install gradio
```

Or install everything at once:

```bash
pip install langchain langchain-community langchain-huggingface langchain-text-splitters sentence-transformers transformers faiss-cpu pypdf gradio
```

---

## ▶️ How to Run

### 1. Open the notebook

Open `Context_Aware_RAG_Chatbot.ipynb` in Google Colab or Jupyter Notebook.

### 2. Install dependencies

Run the installation cell.

### 3. Upload a PDF

Upload any PDF document when prompted.

### 4. Load the document

The chatbot reads all pages from the uploaded PDF.

### 5. Split the document

The document is divided into smaller overlapping chunks for better retrieval.

### 6. Create embeddings

Generate semantic embeddings using:

```
sentence-transformers/all-MiniLM-L6-v2
```

### 7. Build the FAISS vector database

Store all document embeddings for fast similarity search.

### 8. Create the retriever

Retrieve the most relevant chunks for each user query.

### 9. Load the language model

The chatbot uses:

```
TinyLlama/TinyLlama-1.1B-Chat-v1.0
```

### 10. Build the RAG pipeline

Combine the retriever with the language model to answer questions using the uploaded document.

### 11. Launch Gradio

Run the Gradio interface and open the generated public URL to interact with the chatbot.

---

## 📌 Workflow

```
PDF Upload
      │
      ▼
Load PDF
      │
      ▼
Split into Chunks
      │
      ▼
Generate Embeddings
      │
      ▼
Store in FAISS
      │
      ▼
Retrieve Relevant Chunks
      │
      ▼
Generate Response using TinyLlama
      │
      ▼
Display Answer in Gradio Chat Interface
```

---

## 💬 Example Questions

- What is this document about?
- Summarize the document.
- What are the main topics?
- What is the conclusion?
- Who is mentioned in the document?
- Explain the key findings.

---

## 📊 Project Pipeline

1. Upload PDF
2. Load PDF
3. Split into chunks
4. Generate embeddings
5. Store embeddings in FAISS
6. Retrieve relevant chunks
7. Pass retrieved context to the LLM
8. Generate contextual answers
9. Display results in Gradio

---

## 📈 Future Improvements

- Support multiple PDF documents
- Persistent chat history
- True conversational memory
- Source citation with page numbers
- Hybrid search (Keyword + Semantic)
- Support for Word and PowerPoint documents
- Deploy on Hugging Face Spaces
- Docker containerization
- Streamlit web application

---

## 📷 Screenshots

Add screenshots of:

- PDF upload
- FAISS index creation
- Chatbot interface
- Sample conversation
- Gradio application



## ⭐ Acknowledgements

- LangChain
- Hugging Face
- Sentence Transformers
- FAISS
- Gradio
- Google Colab

---

## 🎯 Outcome

This project demonstrates how Retrieval-Augmented Generation (RAG) can be used to build an intelligent chatbot capable of answering questions from uploaded PDF documents using semantic search and Large Language Models. The chatbot improves response relevance by retrieving the most appropriate document chunks before generating answers.
