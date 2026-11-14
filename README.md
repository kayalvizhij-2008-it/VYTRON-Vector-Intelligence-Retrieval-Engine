# VYTRON — Vector Intelligence & Retrieval Engine

<p align="center">
  <strong>Beyond Similarity. Into Intelligence.</strong>
</p>

<p align="center">
  An intelligent knowledge retrieval and AI reasoning platform designed to transform fragmented information into connected, contextual, and actionable intelligence.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-Backend-blue?logo=python" />
  <img src="https://img.shields.io/badge/React-Frontend-61DAFB?logo=react" />
  <img src="https://img.shields.io/badge/TypeScript-Engineering-3178C6?logo=typescript" />
  <img src="https://img.shields.io/badge/FastAPI-API-009688?logo=fastapi" />
  <img src="https://img.shields.io/badge/Qdrant-Vector%20Database-DC382D" />
  <img src="https://img.shields.io/badge/AI-Hybrid%20RAG-8A2BE2" />
</p>

---

## Overview

**VYTRON** is an AI-powered Knowledge Intelligence Platform that goes beyond conventional similarity-based search.

It combines vector retrieval, lexical search, intelligent reranking, retrieval-augmented generation (RAG), knowledge graph concepts, and autonomous research workflows to help users discover relationships, understand information, and generate context-aware responses.

Rather than treating documents as isolated data sources, VYTRON aims to create an interconnected intelligence layer that makes organizational knowledge searchable, explainable, and useful.

## The Vision

Traditional search finds information.

VYTRON aims to understand how information connects.

Its architecture brings together multiple retrieval and reasoning techniques to create a more comprehensive knowledge discovery experience.

## Core Capabilities

### 1. Hybrid Intelligence Retrieval
- Semantic vector search.
- Sparse lexical retrieval using BM25.
- Reciprocal Rank Fusion (RRF).
- Cross-encoder reranking.
- Context-aware retrieval pipelines.

### 2. Agentic RAG Architecture
- Retrieval-augmented answer generation.
- Multi-step research workflows.
- Context-aware reasoning.
- Source-grounded response generation.
- Citation and answer verification.

### 3. Knowledge Graph Intelligence
- Entity and relationship extraction.
- Connected knowledge exploration.
- Multi-hop relationship discovery.
- Context enrichment through related information.

### 4. Trust & Answer Verification
- Transparent TrustScore calculations.
- Retrieval evidence analysis.
- Claim-level verification.
- Citation coverage and answer quality evaluation.

TrustScore is an evidence-based heuristic, not a calibrated probability of correctness.

### 5. Retrieval Observatory
- Retrieval pipeline visibility.
- Search and reranking diagnostics.
- Pipeline execution traces.
- Performance and latency monitoring.

### 6. Evaluation & Analytics
- Precision@K.
- Recall@K.
- Mean Reciprocal Rank (MRR).
- Normalized Discounted Cumulative Gain (nDCG).
- Faithfulness and citation coverage evaluation.
- Retrieval and application analytics.

### 7. Enterprise-Oriented Workspace Management
- Workspace-based data isolation.
- Role-based access control.
- User authentication.
- Document and knowledge management.
- Access management and audit-oriented workflows.

## Technology Stack

| Layer | Technologies |
|---|---|
| Frontend | React, TypeScript, Vite |
| Backend | Python, FastAPI |
| Vector Database | Qdrant |
| Dense Embeddings | Sentence Transformers |
| Sparse Retrieval | Rank-BM25 |
| Reranking | Cross-Encoder |
| Retrieval Fusion | Reciprocal Rank Fusion |
| AI Integration | OpenAI / Anthropic provider architecture |
| Database | SQLite development support; PostgreSQL production integration |
| Caching / Jobs | Redis integration |
| Agent Architecture | LangGraph |
| Visualization | Custom Canvas and WebGL2 components |

## System Architecture

```text
                 VYTRON PLATFORM
                        |
          +-------------+-------------+
          |                           |
     React Frontend              FastAPI Backend
          |                           |
          |                    Application Services
          |                           |
          |          +----------------+----------------+
          |          |                |                |
          |      Ingestion         Retrieval         Agents
          |          |                |                |
          |          |          +-----+-----+          |
          |          |          |           |          |
          |          |        Dense       BM25      Research
          |          |        Search      Search     Workflows
          |          |          |           |          |
          |          |          +-----+-----+          |
          |          |                |                |
          |          |          RRF Fusion             |
          |          |                |                |
          |          |          Reranking              |
          |          |                |                |
          |          +----------> RAG Engine <----------+
          |                           |
          |                    LLM Integration
          |                           |
          +---------------------------+
                                      |
                           Grounded AI Responses
```

## Experience & Interface

VYTRON features a custom dark interface designed around a futuristic knowledge-intelligence aesthetic.

Its visual experience includes:

- NeuralParticleField — adaptive particle visualization.
- CorollaGleam — custom WebGL2 GLSL iridescent glass rendering.
- VytronExperience — layered visual composition with graceful rendering fallbacks.
- Retrieval Observatory.
- Evaluation Lab.
- Command Center.
- Knowledge Graph Explorer.

The original custom visual components are part of the project identity, not generic replacement effects.

## Project Structure

```text
VYTRON/
│
├── backend/
│   ├── routes/
│   ├── services/
│   ├── models/
│   ├── tests/
│   ├── README.md
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── ...
│   └── ...
│
├── docs/
│   └── ARCHITECTURE.md
│
├── backend/
│   └── Dockerfile
│
└── README.md
```

The actual repository structure may include additional modules and configuration files.

## Getting Started

### Prerequisites

- Python 3.11 or compatible project-supported version.
- Node.js and npm.
- Git.
- Qdrant instance for vector database integration.
- An API key for a supported LLM provider when using external AI generation.

### Clone the Repository

```bash
git clone https://github.com/kayalvizhij-2008-it/NEXORA-AI.git

cd NEXORA-AI
```

### Backend Setup

```bash
cd backend

python -m venv venv
```

Activate the virtual environment on Windows:

```powershell
.\venv\Scripts\Activate.ps1
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Configure your local environment using the provided `.env.example` and the backend README.

### Frontend Setup

```bash
cd frontend

npm install
```

Use the project's configured Vite development command to start the frontend.

Refer to the existing backend and frontend documentation for exact startup commands and configuration requirements.

## Configuration

VYTRON supports external infrastructure integrations.

Typical configuration categories include:

- Qdrant endpoint and API authentication.
- LLM provider credentials.
- Database connection.
- Optional Redis connection.
- Frontend backend API endpoint.

Never commit `.env` files, API keys, tokens, or private credentials to version control.

## Security

Security is a core part of VYTRON's architecture.

Existing security mechanisms include:

- Password hashing using PBKDF2-HMAC-SHA256.
- HMAC-based session tokens.
- Workspace isolation.
- Role-based access control.
- Request validation.
- Security response headers.
- API rate limiting.

Production deployment should additionally validate secret management, database security, persistent rate limiting, CORS policies, and operational monitoring.

## Development Status

VYTRON has an implemented application foundation, including its FastAPI backend, React frontend, retrieval services, authentication architecture, and custom visualization components.

The development and integration roadmap includes:

- Live Qdrant infrastructure connection.
- Configured external LLM provider.
- Complete document-to-answer integration testing.
- Production PostgreSQL configuration.
- Optional Redis-based background processing.
- Streaming responses.
- Production deployment and end-to-end verification.

Features that depend on external services should be considered complete only after real integration tests succeed.

## Roadmap

- [x] FastAPI application foundation.
- [x] React and TypeScript frontend foundation.
- [x] Authentication and workspace architecture.
- [x] Hybrid retrieval components.
- [x] Reranking and retrieval fusion components.
- [x] Custom 3D and WebGL visual experience.
- [ ] Fully connected production Qdrant infrastructure.
- [ ] Verified end-to-end grounded RAG workflow.
- [ ] Production PostgreSQL deployment.
- [ ] Background processing and streaming.
- [ ] Complete production deployment.
- [ ] Expanded retrieval and answer evaluation.

## Contributing

Contributions, ideas, architecture discussions, and improvements are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Implement and test your changes.
4. Submit a pull request with a clear explanation.

## Project Identity

**VYTRON — Vector Intelligence & Retrieval Engine**

*Beyond Similarity. Into Intelligence.*

Building a smarter way to search, connect, understand, and use knowledge.

---

<p align="center">
  <strong>VYTRON</strong><br/>
  Intelligent Retrieval. Connected Knowledge. Contextual Reasoning.
</p>
