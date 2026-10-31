# Multimodal Document Intelligence

A document intelligence system designed to process documents containing text and visual information, extract structured information, and retrieve relevant evidence.

## Overview

This project explores multimodal document processing by combining document extraction, OCR/vision integration points, structured information extraction, and evidence-based retrieval.

It provides an application workflow for working with PDF, text, and Markdown documents, with optional OCR and vision adapters.

## Key Features

- PDF, TXT, and Markdown document support.
- PDF text extraction.
- Table extraction support.
- Optional OCR integration.
- Optional vision adapter.
- Structured information extraction.
- Evidence-based retrieval.
- FastAPI application interface.
- Automated tests.

## Architecture

```text
          Document Upload
                 |
                 v
         Document Processing
                 |
          +------+------+
          |             |
          v             v
      Text Parser    Visual Input
          |          OCR / Vision
          |             |
          +------+------+
                 |
                 v
         Structured Extraction
                 |
                 v
          Evidence Retrieval
                 |
                 v
          Extracted Results
```

## Technology Stack

- Python
- FastAPI
- PDF processing
- OCR / vision adapter interfaces
- Structured data extraction
- Retrieval workflows
- Pytest

## Project Structure

```text
multimodal-document-intelligence/
│
├── app/
├── src/
├── tests/
├── data/
├── requirements.txt
├── README.md
└── .gitignore
```

*The actual repository structure takes precedence over this illustrative tree.*

## Installation

```bash
git clone https://github.com/Chanikyaa/multimodal-document-intelligence.git
cd multimodal-document-intelligence

python -m venv .venv
```

Activate the environment:

**Windows**
```bash
.venv\Scripts\activate
```

**Linux/macOS**
```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Running the Application

Start the FastAPI application using the entry point configured in the source code.

For example, if the application exposes `app.main:app`:

```bash
uvicorn app.main:app --reload
```

Open the interactive API documentation:

```text
http://127.0.0.1:8000/docs
```

## Supported Document Types

- PDF
- TXT
- Markdown

## Engineering Concepts Demonstrated

- Document processing pipelines
- Multimodal AI architecture
- OCR and vision integration
- Structured information extraction
- Evidence-based retrieval
- REST API development
- Automated testing

## Current Validation

- Automated tests: **11 passed**.
- ZIP integrity and Python compilation checks passed.
- PDF extraction and retrieval CLI smoke tests passed.

## Limitations

- The mock vision adapter does not interpret image content.
- Live vision-provider benchmarking has not been completed.
- Full scanned-PDF OCR and chart question-answering have not been validated.
- Authentication, tenant isolation, and persistent storage remain areas for improvement.
- Docker and live provider execution have not been verified.

## Future Improvements

- Integrate a real vision-language model.
- Improve OCR for scanned documents.
- Add chart and image understanding.
- Implement persistent document storage.
- Add user authentication and tenant isolation.
- Build a document intelligence dashboard.

## Author

**Palli Chanikya Paidi Balaji**

B.Tech – VIT Chennai (2025)  
M.Tech CSE – AI & Data Science, Mahindra University (2026–2028)

GitHub: [@Chanikyaa](https://github.com/Chanikyaa)

---

*Part of an AI/ML Engineering Portfolio.*
