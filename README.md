# Agentic RAG System

An intelligent Retrieval-Augmented Generation (RAG) system built with LangGraph, featuring a ReAct agent with document retrieval and Wikipedia search capabilities.

## Features

- **Document Ingestion**: Load documents from URLs, PDFs, and text files
- **Vector Store**: FAISS-based semantic search with OpenAI embeddings
- **ReAct Agent**: Intelligent agent that can use retriever and Wikipedia tools
- **Streamlit UI**: Simple web interface for interacting with the system
- **LangGraph Workflow**: Structured RAG pipeline with state management

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
