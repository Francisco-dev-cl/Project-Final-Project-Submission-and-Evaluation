# Project: Final Project Submission and Evaluation

This repository houses a comprehensive full-stack capstone project featuring an end-to-end, multi-tier application architecture that integrates a Model Context Protocol (MCP) server-client system with a polished graphical user web interface.

## 🎯 Project Objective

The goal of this final project is to synthesize advanced backend development with state-of-the-art AI interface patterns. The application pulls together a complete software workflow: raw unstructured text data is loaded and structured, an asynchronous MCP server exposes specific lookup tools over that data, an MCP client manages runtime model queries, and a live web application serves everything up to users through an interactive dashboard.

## 📁 Repository Structure

* **`app.py`**: The main frontend web application layer—built with Gradio—providing user dashboard elements, streaming text boxes, and handling interactive user session routing.
* **`client.py`**: The MCP orchestration client that establishes connections to the context server, translates human requests into semantic commands, and formats data payloads for downstream Large Language Models.
* **`server.py`**: The foundational MCP server component which exposes programmatic tools, handles asynchronous I/O loops, and serves specific context queries over database endpoints.
* **`test.py`**: Validation suite engineered to handle integration testing, check client-server protocol handshakes, and stress-test data extraction handlers.
* **`California-Culinary-Map.txt`**: Complex unstructured source text block containing localized asset, review, and geolocation data.
* **`structured-restaurant-data.json` & `augmented-user-review.json`**: Structured relational JSON databases used as the operational data layers for the server tools.
* **`.gradio/` & `.theia/`**: Hidden environment directories tracking localized workspace cache settings, styling metrics, and system runtime variables.

## 🛠 Technologies Used

* **Interface UI Framework:** Gradio (or Flask/HTML companion views)
* **Protocol Standard:** Model Context Protocol (MCP SDK for Python)
* **Programming Paradigm:** Asynchronous Python (`asyncio`), Functional Tool Building
* **Data Layer & Structures:** JSON, Raw Stream Text Parsing, Key-Value Matrix Indexing

## 🚀 Installation and Execution

### Local Environment Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd Project-Final-Project-Submission-and-Evaluation
   ```

2. **Install all platform and AI dependencies:**
   Make sure you have an active Python environment, then run:
   ```bash
   pip install mcp gradio requests openai asyncio
   ```

3. **Verify infrastructure via the integration test suite:**
   ```bash
   python test.py
   ```

4. **Launch the master web application interface:**
   ```bash
   python app.py
   ```
   Open your browser and navigate to the local hosting url outputted in your console (typically `http://127.0.0.1:7860`).

## 📈 Demonstrated Skills

* **Full-Stack AI Application Engineering:** Seamlessly connecting UI frontends, protocol client layers, asynchronous servers, and relational datasets into a single high-performance software application.
* **Model Context Protocol Implementation:** Advanced understanding of distributed tool calling architectures, data-masking boundaries, and system-to-LLM pipeline standardizations.
* **Production Quality Assurance:** Designing decoupled test scenarios (`test.py`) that reliably pinpoint communication gaps across multi-tier networking stacks.
