🛡️ Intelligent Fraud Detection System (RAG + Llama 3.2 3B)
📌 Project Overview
This repository contains the implementation of an advanced, context-aware Fraud Detection System. Developed as part of the Intel Unnati program, this project leverages a Retrieval-Augmented Generation (RAG) pipeline to analyze and identify fraudulent patterns with high accuracy.

At the core of this system is the Meta Llama 3.2 3B Instruct model. To ensure computational efficiency and optimal memory footprint without sacrificing inference quality, the model integration utilizes a BitsAndBytes (bnb) configuration for advanced quantization.

✨ Key Features
Retrieval-Augmented Generation (RAG): Enhances the LLM's detection capabilities by grounding its reasoning in a domain-specific, localized dataset, minimizing hallucinations and improving factual accuracy.

State-of-the-Art LLM: Utilizes the highly capable Meta Llama 3.2 3B Instruct model for nuanced, step-by-step reasoning on complex fraud indicators.

Memory-Efficient Quantization: Implements BitsAndBytesConfig (4-bit/8-bit precision) to run the pipeline efficiently on consumer-grade or resource-constrained hardware.

Included Dataset: A curated dataset is provided within the repository to facilitate immediate testing, evaluation, and pipeline recreation.

🏗️ System Architecture
Data Ingestion: The provided dataset is parsed, cleaned, and chunked.

Vectorization & Indexing: Text chunks are converted into embeddings and stored in a vector database for semantic search.

Retrieval: Upon receiving a query or transaction log, the system retrieves the most relevant context from the indexed dataset.

Generation & Analysis: The Llama 3.2 3B model, loaded via bnb, synthesizes the retrieved context and the user query to output a definitive fraud analysis and classification.

🚀 Installation & Setup
Prerequisites
Python 3.10 or higher

CUDA-compatible GPU (Recommended for Llama inference)

Hugging Face account and access token (to download Llama 3.2)
