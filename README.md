This project is an interactive Conversational Retrieval-Augmented Generation (RAG) system built using:

📚 LangChain for building LLM pipelines

🧠 Groq LLMs (e.g., Gemma2-9b-It)

📄 Multi-format document loaders (PDF, DOCX, TXT, CSV, Markdown)

📦 Chroma for in-memory vector store

🖥️ Streamlit for a sleek front-end interface

💬 Persistent chat history with session management

🚀 Features
✅ Upload and chat with files (PDF, DOCX, TXT, CSV, Markdown)

✅ Uses RAG pipeline to answer queries using document content

✅ Reformulates follow-up questions with chat history awareness

✅ Custom session-based chat history management

✅ Secure API key input for Groq LLMs

✅ Uses HuggingFace embeddings (all-MiniLM-L6-v2) with Chroma vectorstore

📦 File Support
You can upload any of the following file types:

.pdf

.docx

.txt

.csv

.md

🧰 Tech Stack

Layer	Tool/Library
LLM Backend	Groq API
Embeddings	HuggingFace (all-MiniLM-L6-v2)
RAG Framework	LangChain
Vector Store	Chroma
UI	Streamlit
Chat History	langchain_core.chat_history
🔐 Setup Instructions
1. Clone the repository
bash
Copy
Edit
git clone https://github.com/<your-username>/RAG-QnA-Conversation.git
cd RAG-QnA-Conversation
2. Install dependencies
Create a virtual environment and install from requirements.txt:

bash
Copy
Edit
pip install -r requirements.txt
3. Create a .env file
⚠️ Never commit this file. It's in .gitignore.

env
Copy
Edit
HF_TOKEN=your_huggingface_token
4. Run the Streamlit app
bash
Copy
Edit
streamlit run app.py
🔑 API Keys Required
Groq API Key – You’ll be prompted to enter this in the UI.

Hugging Face Token – Required in .env for embedding model loading.


🧪 Example Workflow
Upload a .pdf, .txt, or .csv file.

Ask a question like: "What is the main idea of the second section?"

Continue the conversation with: "And how does that relate to the conclusion?"

The system reformulates and answers with context from history.

🛡️ Security
Sensitive keys are never committed (.env is ignored).

GitHub secret scanning protects against accidental exposure.

📜 License
MIT License. Feel free to fork and modify.
