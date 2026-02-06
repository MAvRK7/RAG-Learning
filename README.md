# RAG-Learning

# Requirements 

```bash
pip install sentence-transformers faiss-cpu numpy python-dotenv openai mistralai langgraph langchain
```

- python 3 (ive used 3.12)
- imports: os, numpy, faiss, OpenAI
- pip install sentence-transformers faiss-cpu numpy python-dotenv openai mistralai langgraph langchain
- you would need an API Key from openrouter to use the LLM. The LLM used here is the nemotron-3-nano-30b-a3b by NVIDIA, but any LLM works
- Later mistralai has been used as a fall back if openrouter hits the rate-limit
- LanGraph is used to make agentic application better 

# Organization:

1. simple-rag: 
strictly answers only from docs. If query's not in the docs, model says "idk"
2.  agentic-rag: knows when to retrieve and when to answer
3.  langgraph-agent: agent control flow using graohs- LangGraph implementation
