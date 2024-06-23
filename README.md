# RAG for Insurance Document Retrieval (01/2024)
This repository contains a Retrieval-Augmented Generation (RAG) system built in Python for retrieving information from insurance documents stored in PDF format. The system leverages OpenAI's latest embedding model to encode chunked text data and utilizes topic modeling to extract keywords from each document. These keywords are linked to the embeddings of the chunks, providing a broader context for each chunk. The encoded questions are then compared to the chunks by computing the cosine similarity. The top 5 chunks, along with their corresponding keywords, are passed to the GPT-4 model to answer the question.

Features
- PDF Parsing: Extracts text from PDF insurance documents.
- Chunking: Breaks down large documents into manageable text chunks.
- Embedding: Uses OpenAI's latest embedding model to encode text chunks.
- Topic Modeling: Generates keywords for each document to provide additional context.
- Cosine Similarity: Compares encoded questions with text chunks to identify the most relevant chunks.
- Answer Generation: Uses GPT-4 to generate answers based on the top 5 relevant chunks and their keywords.
