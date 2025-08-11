# ADGM Corporate Agent — Streamlit Demo (with Google Gemini integration)

This demo app accepts `.docx` uploads, classifies document types (AoA, MoA, UBO, Register, etc.), verifies a Company Incorporation checklist, runs red-flag checks, uses a local RAG pipeline with Chroma + Sentence-Transformers, and calls Google Gemini for ADGM-specific legal compliance analysis.

---

## ✨ Features
- Safe handling when RAG reference folder is missing.
- Checks for existing Chroma collection before retrieval.
- Handles `None` or empty Gemini responses without crashing.
- Accurate document classification (supports abbreviations).
- Better placement of review notes in `.docx` files.
- More accurate process detection (requires at least 2 core documents).
- Structured JSON report with severity tagging (`critical`, `major`, `medium`, `minor`).

---

## 🛠 Setup

### 1. Environment
- Python **3.9+** is required.
- Create and activate a virtual environment:
  ```bash
  python -m venv venv
  source venv/bin/activate  # macOS/Linux
  venv\Scripts\activate     # Windows
