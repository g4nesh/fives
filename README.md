# Fives

Fives is an open-sourced desktop application that leverages Retrieval-Augmented Generation (RAG) and vector search to make your local files truly searchable. Instead of just relying on filenames or metadata, Fives indexes file contents and lets you query them in natural language — just like talking to your computer.

✨ Features

File Indexing with RAG – Builds embeddings for your documents and stores them in a local vector database.

Natural Language Search – Search across all your files with questions like “Show me the report where I mentioned glucose sensors last month”.

Cross-File Summarization – Summarize information across multiple documents instantly.

Privacy-First – All processing and indexing happens locally on your machine. Nothing leaves your computer.

Desktop Integration – Runs as a lightweight app that plugs into macOS Finder or Windows File Explorer.

Multi-format Support – Works with PDFs, Word docs, text files, CSVs, and more (extensible to custom formats).

🔧 Tech Stack

Frontend: Electron (desktop shell)

Backend: Python (FastAPI or Flask)

Vector Database: FAISS / ChromaDB / Milvus (configurable)

Embeddings: OpenAI, HuggingFace, or local models (user-selectable)

RAG Pipeline: Combines vector search retrieval with a language model to generate contextual answers.


📂 How It Works

Indexing – The app scans selected folders, extracts text from files, generates embeddings, and stores them in a local vector DB.

Retrieval – When you ask a question, Fives retrieves the most relevant documents.

Augmented Generation – The context is passed into an LLM (local or API-based), which crafts an answer grounded in your own files.

🛠 Roadmap

 Cross-platform builds (macOS, Windows, Linux)

 Advanced file filtering (date, type, size)

 Real-time indexing

 Plugin system for custom file parsers

 Offline mode with small local LLMs

🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change.

