# System Architecture

The architecture of **PaperPilot AI** is designed to provide highly accurate, verifiable, and context-aware responses to complex academic queries. It seamlessly integrates IBM's enterprise AI offerings with a custom Retrieval-Augmented Generation (RAG) pipeline.

## High-Level Architecture Flow

1. **User Interface (Frontend)**
   - The user interacts with the beautifully crafted HTML/CSS frontend.
   - The user inputs a query or prompt into the embedded IBM watsonx chat widget.

2. **IBM watsonx Orchestrate**
   - Acts as the central orchestration layer.
   - Routes the user's intent to the appropriate internal AI agents and skills.
   - Manages state, conversation history, and security.

3. **IBM Granite Models**
   - The core Large Language Model (LLM) engine.
   - Optimized for complex reasoning, summarization, and data extraction.
   - Receives the structured prompt and context from the orchestrator.

4. **RAG Pipeline (Retrieval-Augmented Generation)**
   - When a user asks a factual question or requests a literature review, the RAG system kicks in.
   - It converts the user's query into vector embeddings.
   - Performs semantic search across the **Scientific Knowledge Base**.
   - Retrieves the top `K` most relevant research paper chunks and citation metadata.

5. **Knowledge Base**
   - A vector database containing parsed and embedded peer-reviewed papers, academic journals, and textbooks.

6. **Response Synthesis**
   - The retrieved context is injected into the IBM Granite prompt.
   - Granite synthesizes a comprehensive response, ensuring that all claims are grounded in the retrieved documents.
   - The response is streamed back through watsonx Orchestrate to the user's browser.
