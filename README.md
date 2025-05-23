# 📄GEN AI - POWERED PDF CHATBOT: INTELLIGENT DOCUMENT INTERACTION USING STREAMLIT,LLM.

A simple Streamlit web app that allows you to **chat with your PDF documents** using **Large Language Models (LLMs)**. Ask natural language questions and get accurate, context-aware answers from your PDFs—no manual searching required!

---

## 🚀 Features

- Upload one or more PDF files.
- Ask questions in plain English.
- Receive responses directly from your document content.
- Interactive chat interface using Streamlit.
- Uses Hugging Face models and FAISS for semantic search.

---

## 🧠 Example Use Case

In the example below, the user asked who the guest was in episode 791 of the Super Data Science podcast hosted by Jon Krohn:

<img width="1179" alt="Chat Example" src="https://github.com/byiliakarelin/Chat-With-Your-Favorite-PDF/assets/132295797/2180a1e6-be0f-4c85-8741-967201c2933e">

---

## 📽️ Screen Recording / Demo

[Click here or watch below to see the app in action!](https://github.com/user-attachments/assets/7de0fdf5-9479-4f19-8558-1e084c421ea6)


---

## ⚙️ How It Works

### 📄 Text Extraction

Text is extracted from each page of the uploaded PDF(s) using PDF parsing libraries.

### ✂️ Text Chunking

The extracted text is split into manageable chunks with a specified chunk size and overlap. This helps improve processing accuracy and enables effective embedding.

### 🧠 Embeddings & Vector Storage

Each chunk is converted into embeddings using a sentence transformer model hosted on Hugging Face. These embeddings are stored in a FAISS vector index to enable efficient semantic search.

### 🔗 Conversation Chain Setup

A conversational retrieval chain is initialized, combining:
- Context-aware prompt templates
- The FAISS-based retriever
- A Hugging Face language model
- Memory buffer for preserving chat history

This enables dynamic and coherent conversations based on the document’s content.

---

## 🛠️ Tech Stack

| Technology               | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| 🧠 Generative AI         | Powers natural language generation and understanding.                      |
| 🤗 Hugging Face API      | Accesses pretrained LLMs via secure API token.                             |
| 📚 LLM (Large Language Model) | Processes PDF content to generate context-aware responses.             |
| 🔍 FAISS                 | Efficient similarity search using vector embeddings from PDF content.       |
| 🌐 Streamlit             | Builds an interactive web-based UI for chatting with your PDF.             |
| 🔐 Environment Variables | Stores secrets like Hugging Face API token securely in a `.env` file.       |


## 🖥️ User Interface

The app uses Streamlit for its front-end:

- The main chat area displays the conversation between the user and the bot.
- A sidebar allows users to upload multiple PDF files.
- Once the “Process” button is clicked:
  - The PDF text is extracted.
  - The text is split into chunks.
  - Embeddings are generated and indexed.
  - A conversation chain is initialized.

Users can then ask questions about the PDF, and the application responds using the knowledge embedded from the document.

---

## 📋 Chat History

- Stored using Streamlit session state.
- Displayed in reverse chronological order (latest message first).
- Formatted using custom HTML/CSS templates for a chat-like experience.

---

## ✅ Setup Instructions

To run the project locally:

1. Clone the repository.
2. Install the required packages listed in `requirements.txt`.
3. Run the Streamlit app using `streamlit run webapp.py`.
4. Upload PDF files in the sidebar and start chatting!

---

## 🔐 Notes

- API keys or model tokens (if required) should be securely stored in a `.env` file.
- You can modify the model, chunk size, or other parameters based on your needs.
- The app is adaptable to many use cases including academic research, meeting transcripts, books, and more.

---
## 👤 Author Profile

### 🚀 **Mulinti Rohith Naidu**

🤖 **LLM Engineer** | 📚 **PDF Chatbot Builder**

📧 **Email**: [mulintirohan159@gmail.com](mailto:mulintirohan159@gmail.com)  
🔗 **LinkedIn**: [Visit Profile](https://linkedin.com/in/rohith-naidu-16a2004mar)

---

> Passionate about building decentralized solutions and innovative tech projects.


**Happy PDF Chatting!** 🤖📚
