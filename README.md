# Document Copilot: SEC Filing Research Assistant

## Overview

This project is a **full-stack Generative AI** application designed for deep equity research. It enables users to perform **Retrieval-Augmented Generation (RAG)** over SEC filings to obtain grounded answers with citations and chat history.

## Tech Stack

*   **Backend:** FastAPI, Python
*   **Database:** Supabase (PostgreSQL with `pgvector` for vector storage)
*   **Frontend:** React, TypeScript, Tailwind CSS, shadcn/ui
*   **AI/Orchestration:** OpenAI API, Pydantic, Docling (for document ingestion)
*   **Deployment:** Railway

## Architecture Highlights

*   **Ingestion Pipeline:** Uses Docling to convert HTML filings into clean Markdown, followed by hierarchical chunking and embedding generation.
*   **Hybrid Search:** Combines **semantic vector search** (using `pgvector`) with **full-text search** for keyword relevance.
*   **Agentic Workflow:** Utilizes a validator pattern to ensure citations are grounded and to maintain high-quality, hallucination-resistant responses.

## Key Features

*   **Citations:** Inline references that link back to the specific source chunks.
*   **Chat Persistence:** History tracking per user session.
*   **Authentication:** Secure user login via Supabase Auth.

## Project Reference

This implementation is based on the guide provided by Dave Ebbelaar: [Build a Full-Stack GenAI Project in 4 Hours (FastAPI, React, Supabase)](https://www.youtube.com/watch?v=kYJj8w7u_y0)
