# LebLens

LebLens is an AI-powered medical lab report analyzer that helps users upload a PDF or image of a blood test report, extract the values, and receive clear, plain-language explanations of each result.

The project is designed to make routine lab interpretations more accessible to patients, caregivers, and non-specialists by turning technical medical values into understandable guidance.

## Why this project exists

Medical reports often contain dense, technical labels and ranges that can be difficult to interpret without clinical context. LebLens aims to bridge that gap by combining:

- OCR / document parsing for scanned PDFs and images
- Structured extraction of lab values and units
- AI-based explanation of each parameter in everyday language
- A simple interface for uploading reports and reviewing results

## Core features

- Upload blood report PDFs or images
- Extract test values and reference ranges
- Identify abnormal or borderline readings
- Explain each test in plain language
- Provide a readable summary of a patient’s overall report
- Support a web app frontend with a Python backend

## Tech stack

- Frontend: React
- Backend: FastAPI
- Database: SQLite
- AI / analysis layer: LLM-powered interpretation and document processing
- File input support: PDF and image uploads

## High-level architecture

- Frontend React app for upload, rendering, and user interaction
- FastAPI API for request handling and business logic
- SQLite database for storing application state, reports, and metadata
- AI inference layer for interpreting extracted lab values and generating explanations

## Typical workflow

1. User uploads a blood report PDF or image.
2. The backend processes the file and extracts lab values.
3. The extracted values are normalized and compared against reference ranges.
4. AI interprets the result and provides a plain-language explanation.
5. The frontend displays the report in a clean, understandable format.

## Project goals

- Make report interpretation more accessible
- Reduce ambiguity in routine lab results
- Create a usable, patient-friendly interface
- Combine document extraction with health-focused AI explanation

## Repository structure

This repository currently acts as the foundation for the application. Suggested structure as the project grows:

- `frontend/` — React application
- `backend/` — FastAPI services
- `database/` — SQLite schema and migration files
- `docs/` — project documentation and design notes
- `tests/` — automated validation for parsing and analysis logic

## Getting started

### Prerequisites

- Node.js and npm
- Python 3.10+
- pip
- Virtual environment tooling

### Example setup

```bash
# frontend
cd frontend
npm install
npm run dev

# backend
cd backend
python -m venv .venv
source .venv/bin/activate   # or .venv\Scripts\activate on Windows
pip install -r requirements.txt
uvicorn app.main:app --reload
```

## Notes

This repository is currently focused on the concept and application architecture for an AI medical report analyzer. As the project develops, the README can be expanded with deployment instructions, API documentation, and example screenshots.

## License

This project does not currently declare a license. If you plan to publish or distribute it publicly, consider adding an open-source license.
