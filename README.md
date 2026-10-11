# Accenture earnings RAG — Version 1

# Using Publicly availabe info such as Press Releases

Minimal LlamaIndex Q&A application using three Accenture FY2026 quarterly earnings PDFs.

## Requirements

- Python 3.11 or 3.12
- Groq. API key with available API credits (You can swap it with openai)

## Setup

```
cd qa_RAG
py -3.11 -m venv .venv
Activate it
python -m pip install -r requirements.txt
Copy-Item .env.example .env
notepad .env
python app.py
```

## Test questions

1. What was Accenture's Q2 FY2026 revenue? Which page supports it?
2. Compare Q1 and Q2 FY2026 revenues.
3. What was the Q2 FY2026 operating margin?
4. What was the Q2 FY2026 full-year revenue growth guidance?
5. What was Accenture's FY2027 Q4 revenue? (should say insufficient evidence)

## Limitations

- PDF table text extraction and semantic retrieval can produce inaccurate financial comparisons.
