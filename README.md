# Enterprise-RAG-Support-System

## Local Hugging Face models

This project uses Hugging Face models for embeddings and chat generation:

- Embeddings: `sentence-transformers/all-MiniLM-L6-v2`
- Chat: `TinyLlama/TinyLlama-1.1B-Chat-v1.0`

Set Pinecone credentials in `.env`:

```env
PINECONE_API_KEY=
PINECONE_INDEX_NAME=it-support-rag
PINECONE_NAMESPACE=it-company-kb
```

You can replace the model names in `.env` with other compatible Hugging Face models:

```env
EMBEDDING_MODEL=sentence-transformers/all-MiniLM-L6-v2
HUGGINGFACE_MODEL=TinyLlama/TinyLlama-1.1B-Chat-v1.0
```

An optional Hugging Face token enables higher Hub rate limits:

```env
HF_TOKEN=hf_your_token
```