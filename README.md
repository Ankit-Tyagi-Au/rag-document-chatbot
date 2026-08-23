# Document Q&A System using RAG

A document question-answering system that uses Retrieval-Augmented Generation (RAG) to answer questions based on the content of a PDF document. Currently loaded with a sample document — the Universal Declaration of Human Rights. Click "Ingest the Data," then ask questions about it — the AI retrieves relevant sections and generates accurate answers based on the document's content.

## What it does

1. Reads a PDF document and splits it into chunks
2. Converts those chunks into embeddings using Google's Generative AI
3. Stores them in a FAISS vector database for fast retrieval
4. When you ask a question, retrieves the most relevant chunks
5. Uses Groq's LLM to generate an answer based only on that retrieved content

## Tech Stack

- **Streamlit** – web interface
- **LangChain** – connects the retrieval and generation pipeline
- **Google Generative AI (Gemini)** – document embeddings
- **Groq (Llama models)** – answer generation
- **FAISS** – vector similarity search

## How to run it

1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Add your API keys to a `.env` file:
4. Run the app: `streamlit run app.py`
5. Click "Ingest the Data into Vector Store", then ask a question

## About this project

This project was set up, debugged, and deployed by me as part of my hands-on learning toward becoming an AI/ML Engineer. It's originally based on a RAG tutorial project, which I extended by fixing several outdated dependencies and deprecated model references to get it working with current library versions.

**Built by:** Ankit
**Connect:** [LinkedIn](https://www.linkedin.com/in/ankittyagi-ai/)

