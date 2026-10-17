# 🛡️ Enterprise Knowledge Intelligence Platform (Advanced RAG)

An enterprise-grade, production-ready Advanced Retrieval-Augmented Generation (RAG) ecosystem built with a completely decoupled microservices architecture. The platform combines a high-performance **Python FastAPI backend** orchestrated via **LangGraph agentic reasoning layers**, and a responsive, interactive **Streamlit frontend** secured by a cloud-persistent **Neon PostgreSQL** database cluster.

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://advanced-rag-intelligence.streamlit.app)
[![FastAPI Backend](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=FastAPI&logoColor=white)](https://enterprise-rag-backend-fhzm.onrender.com)
[![Database: Neon PostgreSQL](https://img.shields.io/badge/Database-Neon_PostgreSQL-00e599?style=flat&logo=postgresql&logoColor=white)](https://neon.tech)

---

## ⚡ Core Architectural Milestones & Features

### 🧠 Agentic RAG & Contextual Grounding Core
* **LangGraph Orchestration:** Utilizes state-machine graphs to power structured, multi-turn dialogue agents with state memory.
* **Hallucination Mitigation:** Enforces rigid vector-space grounding boundaries; answers are strictly anchored to verified document contexts.
* **Hybrid Search Foundations:** Tracks text alignment across index mappings, matching specialized document contexts (SOPs, technical matrices) while generating automated source citation strings.

### 🛡️ Hardened Enterprise Access Governance (RBAC)
* **Clearance Isolation:** Segregates application layers completely into structured `User` and `Admin` permissions workspaces.
* **Cryptographic Token Provisioning:** Includes an administrative verification workflow utilizing live, single-use, cryptographically generated token strings for secure new administrator sign-ups.
* **Executive Console Overrides:** Powers privileged administrative root mutations, providing live user account revocation matrices and targeted database password override fields.

### 🗄️ Resilient Lifespan Cluster Data Layers
* **Neon Cloud Synchronization:** Fully integrated with a serverless cloud PostgreSQL database cluster, ensuring robust relational data storage and complete defense against ephemeral cloud server resets.
* **Race Condition Eradication:** Developed using modern FastAPI asynchronous lifespan context controllers to ensure the platform conducts patient connection pools and schema creation sequences without falling back prematurely to transient files.
* **Memory-Decoupled Processing:** Ingests documents, session records, and vector properties straight into live SQL tables, eliminating local file storage footprints.

### 📊 System Telemetry & Analytical Visibility
* **Knowledge Gap Intelligence:** Automatically flags and stores ungrounded client inputs, providing administrators with clean metadata tables detailing specific operational information deficits.
* **Visual Telemetry Dashboarding:** Connects analytical API metrics to frontend Plotly Express modules, rendering line performance distributions and file allocation pie chart tracking arrays.

---

## 🏗️ System Execution Blueprint

```text
    ┌─────────────────────────┐               ┌────────────────────────┐
    │    Streamlit UI         │  REST HTTP    │    FastAPI Backend     │
    │  (Frontend Web App)     ├──────────────►│    (API Core Hub)      │
    └───────────┬─────────────┘   Payloads    └───────────┬────────────┘
                │                                         │
                ▼                                         ▼
     Custom CSS UI Injection                    LangGraph Agentic Core
     JavaScript Field Validator                 Enterprise Guardrail Hooks
                │                                         │
                └───────────────► 💾 ◄────────────────────┘
                          Neon PostgreSQL Cloud
                        (Persistent Database Vault)

# Enterprise Knowledge Intelligence Platform

An AI-powered Enterprise Knowledge Intelligence Platform built using Retrieval-Augmented Generation (RAG). The system helps users retrieve relevant information from enterprise documents and generate context-aware answers.

## Features

- **Retrieval-Augmented Generation (RAG):** Generates answers grounded in retrieved document content.
- **AI Agent Workflow:** Uses LangGraph to orchestrate the retrieval and reasoning process.
- **FastAPI Backend:** Provides APIs for application functionality.
- **Streamlit Frontend:** Provides an interactive user interface.
- **Role-Based Access Control (RBAC):** Separates user and administrator permissions.
- **PostgreSQL Integration:** Supports persistent relational data storage.
- **Analytics Dashboard:** Displays application metrics and knowledge gaps.

## Tech Stack

- Python
- FastAPI
- Streamlit
- LangGraph
- Retrieval-Augmented Generation (RAG)
- PostgreSQL
- Vector database / ChromaDB
- Docker Compose

## Project Structure

```text
enterprise-rag-intelligence/
├── backend/             # Backend API and application logic
├── frontend/            # Streamlit user interface
├── chroma_db/           # Vector database files, if required
├── docker-compose.yml   # Docker service configuration
├── test_key.py          # Key/configuration test utility
└── README.md            # Project documentation
```

## Prerequisites

Install the following before running the project:

- Python 3.10 or another version supported by the project dependencies
- Git
- Docker Desktop (if using Docker Compose)
- Access to any required API provider
- PostgreSQL database credentials, if required

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/enterprise-rag-intelligence.git
cd enterprise-rag-intelligence
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Configure environment variables

Check the backend configuration and example environment files. Create the required `.env` file in the location expected by the application.

Add the required database URL, API keys, and other settings based on the project's configuration.

**Security:** Never commit API keys, passwords, database credentials, or `.env` files.

### 3. Install dependencies

Inspect the backend and frontend folders for `requirements.txt`, `pyproject.toml`, or other dependency files. Install the dependencies specified by the project.

For a `requirements.txt` file, run:

```bash
python -m pip install -r requirements.txt
```

Run this command from the directory containing that file.

### 4. Start the application

Refer to the backend and frontend instructions and the Docker Compose configuration to determine the correct startup commands.

If Docker Compose is configured for the application, you can try:

```bash
docker compose up --build
```

Use the URLs and ports configured by the project to access the application.

## Troubleshooting

- **ModuleNotFoundError:** Check that you installed dependencies in the correct Python environment.
- **Database connection error:** Verify the database URL, credentials, and network access.
- **API key error:** Confirm that the required environment variables are configured.
- **Port already in use:** Stop the process using the port or configure another available port.
- **Docker errors:** Ensure Docker Desktop is running and the Compose configuration is valid.

## Future Improvements

- Expand document ingestion and retrieval support.
- Improve evaluation of retrieval quality and answer accuracy.
- Enhance monitoring, testing, and deployment automation.

## Disclaimer

This project is intended for educational and development purposes. Review security settings and validate the implementation before using it with sensitive enterprise information.
