# Agentic RAG System

An intelligent Retrieval-Augmented Generation (RAG) system built with LangGraph, featuring a ReAct agent with document retrieval and Wikipedia search capabilities.

## Features

- **Document Ingestion**: Load documents from URLs, PDFs, and text files
- **Vector Store**: FAISS-based semantic search with OpenAI embeddings
- **ReAct Agent**: Intelligent agent that can use retriever and Wikipedia tools
- **Streamlit UI**: Simple web interface for interacting with the system
- **LangGraph Workflow**: Structured RAG pipeline with state management

## Setup

1. Clone the repository:
```bash
git clone <your-repo-url>
cd ragdemo
```

2. Install dependencies:
```bash
pip install -r requirements.txt
# or with uv
uv sync
```

3. Set up environment variables:
```bash
cp .env.example .env
# Edit .env and add your OpenAI API key
```

4. Add your documents to the `data/` folder (PDFs, text files) or update URLs in `src/config/config.py`

## Usage

### Command Line
```bash
python main.py
```

### Streamlit Web UI
```bash
streamlit run streamlit_app.py
```

## Project Structure

```
├── main.py                 # CLI entry point
├── streamlit_app.py        # Web UI
├── src/
│   ├── config/            # Configuration
│   ├── document_ingestion/ # Document loading & processing
│   ├── graph_builder/     # LangGraph workflow
│   ├── node/              # Graph nodes (retriever, ReAct agent)
│   ├── state/             # State definitions
│   └── vectorstore/       # FAISS vector store
├── data/                  # Your documents (gitignored)
└── requirements.txt
```

## Requirements

- Python 3.13+
- OpenAI API key

## License

MIT
