# User Workflow

This document outlines the step-by-step journey of a researcher using **PaperPilot AI**.

## 1. Discovery and Inquiry
- The user lands on the PaperPilot AI portal and navigates through the digital research ecosystem.
- The user clicks "Launch PaperPilot AI" to activate the IBM watsonx Orchestrate agent.
- The user inputs a complex research question, e.g., *"Compare the methodologies used in the top 3 papers regarding Quantum Error Correction from 2023."*

## 2. Intent Recognition & Routing
- IBM watsonx Orchestrate analyzes the input and identifies the intent (Methodology Comparison).
- It triggers the specific RAG skill associated with retrieving full-text academic papers.

## 3. Context Retrieval
- The query is vectorized and searched against the Scientific Vector Database.
- The system retrieves relevant chunks of text from recent Quantum Error Correction papers, including abstract, methodology, and results sections.

## 4. AI Synthesis via Granite
- The retrieved context is passed to the **IBM Granite** foundation model.
- Granite processes the text, compares the experimental setups, identifies differences, and structures the output into a readable comparative format.

## 5. Output Delivery & Citation
- The generated response is delivered to the user in the chat interface.
- Crucially, the response includes inline citations and links back to the original source papers, allowing the user to verify the AI's claims.
