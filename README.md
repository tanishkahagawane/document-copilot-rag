# fullstack-ai-story-builder

This project is a full-stack interactive storytelling platform built with **FastAPI** (backend) and **React** (frontend). It utilizes **Large Language Models (LLMs)** to dynamically generate branching adventure stories based on user-provided themes.

## Project Overview

*   **Backend:** Built with *FastAPI*, featuring asynchronous job processing, database integration with *SQLAlchemy*, and structured data models using *Pydantic*.
*   **AI Integration:** Uses *LangChain* and *OpenAI* to generate creative, multi-path narratives with winning/losing outcomes.
*   **Frontend:** A responsive *React* interface for story input, state management, and navigation through story nodes.
*   **Deployment:** Designed for deployment via platforms like *Choreo*.

## Key Features

*   **Dynamic Generation:** AI-powered story creation based on custom themes.
*   **Branching Paths:** Multiple story nodes with player-driven choices.
*   **Background Processing:** Asynchronous story generation using background tasks to manage LLM latency.
*   **Data Persistence:** Relational database storage for stories, nodes, and session status.

## Getting Started

### Prerequisites

*   Python (managed via *uv*)
*   Node.js
*   OpenAI API Key

### Installation

1.  Clone the repository:
    bash
    git clone https://github.com/techwithtim/Choose-Your-Own-Adventure-AI

2.  Setup the backend dependencies using *uv*.

3.  Configure your environment variables, specifically the `OPENAI_API_KEY`.

4.  Follow the provided build instructions for both the frontend and backend to launch the application.

## Documentation & Credits

This project was built as a full-stack tutorial by *Tech With Tim*. Reference : https://www.youtube.com/watch?v=_1P0Uqk50Ps&t=5s
