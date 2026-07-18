# PaperPilot AI
![IBM watsonx](https://img.shields.io/badge/Powered%20by-IBM%20watsonx-0f62fe?style=for-the-badge&logo=ibm)
![IBM Granite](https://img.shields.io/badge/Model-IBM%20Granite-0f62fe?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)

## Project Overview
PaperPilot AI is an immersive, AI-powered academic research assistant built to revolutionize the way researchers navigate scientific knowledge. Leveraging IBM watsonx Orchestrate and IBM Granite Models, the platform provides automated literature reviews, research gap detection, and methodology comparisons through an elegant, high-end minimalist interface.

## Problem Statement
The volume of academic publications has grown exponentially, making it increasingly difficult for researchers to stay current, synthesize findings, and identify true research gaps. Manual literature reviews take weeks, and cross-referencing methodologies is prone to human error, ultimately slowing down the pace of scientific innovation.

## Features
- **Research Paper Summarization**: Instantly distill complex research papers.
- **Literature Reviews**: Automatically generate comprehensive reviews comparing multiple sources.
- **Research Gap Analysis**: Pinpoint unexplored territories to formulate novel hypotheses.
- **Methodology Comparison**: Side-by-side analysis of experimental setups.
- **Knowledge Discovery**: Navigate complex citation graphs to uncover hidden connections.

## Technology Stack
- **Frontend**: Custom HTML5, CSS3 (Glassmorphism), Vanilla JavaScript
- **AI Orchestration**: IBM watsonx Orchestrate
- **LLM Foundation**: IBM Granite Models
- **Information Retrieval**: Retrieval-Augmented Generation (RAG) Architecture

## Architecture Overview
Our system utilizes a conversational AI agent integrated via **IBM watsonx Orchestrate**. When a user submits an inquiry, the query is processed by **IBM Granite Models** utilizing a **RAG** pipeline connected to a vast scientific knowledge base. 

For detailed diagrams and component breakdowns, see our [Documentation](docs/).

## Installation & Setup
1. Clone the repository: 
   ```bash
   git clone https://github.com/harshad-bgt/paperpilot.git
   ```
2. Navigate to the project directory:
   ```bash
   cd paperpilot
   ```
3. Launch `index.html` in any modern web browser.
4. No external backend servers or build steps are required to view the frontend interface or use the embedded Watsonx agent.

## Usage
- Scroll through the beautifully designed landing page to explore the digital research ecosystem.
- Click the **Launch PaperPilot AI** button to seamlessly scroll to the embedded IBM Watsonx chat widget at the bottom of the page.
- Interact with the AI assistant to ask questions about research methodologies, summarize topics, or generate literature reviews.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
