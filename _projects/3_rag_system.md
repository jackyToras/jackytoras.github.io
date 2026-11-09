---
layout: page
title: askPDF
description: FastAPI, LangChain, ChromaDB, Ollama, Python, React.js, Tailwind CSS
importance: 3
category: work
github: https://github.com/jackyToras/askPDF
---

askPDF is a retrieval-augmented generation application for question answering over PDF and DOCX documents. It combines a FastAPI backend with LangChain, ChromaDB, and a local Ollama language model, with a responsive React and Tailwind CSS interface.

**Document processing and retrieval:** Documents are split into 500-character chunks with 50-character overlap. Their embeddings are stored in ChromaDB, where each question retrieves the top five matches by cosine similarity to provide relevant context for answer generation.

**Multi-user chat:** Uploads and queries are isolated by user ID, with persistent chat history for each user.

**Web interface:** The React and Tailwind CSS frontend provides a responsive chat experience with Markdown rendering and a timeout-aware REST client for multipart uploads and chat requests.
