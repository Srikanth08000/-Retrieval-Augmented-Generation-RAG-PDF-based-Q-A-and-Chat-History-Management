# 📚 PDFChatRAG - Conversational AI with PDFs & Chat History

## 📖 Project Description
**PDFChatRAG** is a **Conversational AI Assistant** that allows users to **upload PDFs, ask questions, and retrieve intelligent answers** while keeping a chat history. It is built using **Streamlit, LangChain, and Groq API** for efficient retrieval-augmented generation (RAG).

This application uses **open-source language models** and **vector embeddings** to extract meaningful insights from documents, making it perfect for **researchers, students, professionals, and anyone looking for an AI-powered document assistant**.

---

## ✨ Features
✅ **Upload & Chat with PDFs** – Upload multiple PDFs and extract meaningful answers.  
✅ **Retrieval-Augmented Generation (RAG)** – Combines search and AI-generated answers for **accurate responses**.  
✅ **Session-Based Chat History** – Keeps track of previous conversations within a session.  
✅ **Multiple Model Support** – Uses Groq's `Gemma2-9b-It` LLM model for responses.  
✅ **Customizable Query Processing** – Reformulates questions based on chat history.  
✅ **Built with Open-Source Models** – Ensuring **transparency & flexibility**.

---

## 🛠️ Technology Stack
- **[Streamlit](https://streamlit.io/)** - Interactive UI for chatting with PDFs  
- **[LangChain](https://www.langchain.com/)** - Framework for LLM orchestration  
- **[Groq API](https://groq.com/)** - Powerful LLM inference  
- **[Hugging Face Embeddings](https://huggingface.co/)** - Text vectorization  
- **[ChromaDB](https://github.com/chroma-core/chroma)** - Embedding-based retrieval  
- **[PyPDFLoader](https://pypdf2.readthedocs.io/)** - Extracts text from PDFs  
- **[dotenv](https://pypi.org/project/python-dotenv/)** - Loads environment variables  

---

## 🚀 Installation Guide

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/your-username/pdfchatrag.git
cd pdfchatrag
2️⃣ Install Dependencies
Ensure you have Python 3.8+ installed. Run:

bash
Copy
Edit
pip install -r requirements.txt
3️⃣ Set Up API Keys
You'll need API keys for Groq and Hugging Face.

🔑 Generate Groq API Key
Go to Groq API
Sign up or log in.
Navigate to API Keys.
Click Create New API Key.
Copy and save it for later.
🔑 Generate Hugging Face API Key
Go to Hugging Face
Sign up or log in.
Click New API Token and copy it.
4️⃣ Set Up Environment Variables
Create a .env file in your project directory and add:

ini
Copy
Edit
HF_TOKEN=your_huggingface_api_key
GROQ_API_KEY=your_groq_api_key
⚠️ Never share or expose your API keys publicly! Add .env to .gitignore:

bash
Copy
Edit
echo ".env" >> .gitignore
🎮 How to Run the Application
Run the Streamlit app:

bash
Copy
Edit
streamlit run app.py
🖥️ Application Interface
1️⃣ Upload PDFs → Click "Choose A PDF file" to upload your document.
2️⃣ Enter your API Key → Provide your Groq API key for processing.
3️⃣ Ask Questions → Type your question, and the chatbot will provide an answer.
4️⃣ Chat History → Maintains a session-based history for better conversation flow.

📚 Example Usage
📌 Question:
plaintext
Copy
Edit
What is LangChain?
🔹 Response:

plaintext
Copy
Edit
LangChain is a framework for building applications with large language models (LLMs) through composability.
📌 Question:
plaintext
Copy
Edit
Summarize the benefits of using open-source language models.
🔹 Response:

plaintext
Copy
Edit
Open-source models provide transparency, flexibility, and control, ensuring data security and reducing dependency on proprietary solutions.
📦 Requirements
🔹 Python Dependencies
Install the required libraries using pip:

bash
Copy
Edit
pip install streamlit langchain langchain_chroma langchain_groq \
    langchain_community langchain_core langchain_huggingface \
    langchain_text_splitters langchain_community.document_loaders \
    chromadb pypdf python-dotenv
🔹 requirements.txt File
Save this file in the project directory:

txt
Copy
Edit
streamlit
langchain
langchain_chroma
langchain_groq
langchain_community
langchain_core
langchain_huggingface
langchain_text_splitters
langchain_community.document_loaders
chromadb
pypdf
python-dotenv
To install dependencies, run:

bash
Copy
Edit
pip install -r requirements.txt
🔹 .env File (Environment Variables)
Save this file in your project directory:

ini
Copy
Edit
HF_TOKEN=your_huggingface_api_key
GROQ_API_KEY=your_groq_api_key
⚠️ Important: Replace the placeholders with your actual API keys.

🧩 Customization Options
Change Language Model: Modify the ChatGroq instance to use a different model.
Enhance Prompt Engineering: Adjust system prompts for better response quality.
Add More File Types: Extend the loader to support TXT, DOCX, etc.
Integrate External APIs: Fetch additional data from knowledge bases or APIs.
🛡️ Security Best Practices
✔️ Do not hardcode API keys – Always use environment variables.
✔️ Avoid exposing sensitive data – Do not print or log API keys.
✔️ Use .gitignore – Ensure .env is ignored in version control.
