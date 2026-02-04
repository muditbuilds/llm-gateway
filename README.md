# LLM Gateway

A proxy service that sits between applications and LLM providers.

## Features (Planned)

- Route requests to different models (GPT-4 for complex, GPT-4o-mini for simple)
- Cache identical prompts
- Retry logic with fallback providers
- Rate limiting per API key
- Token counting and cost tracking
- Request/response logging

## Setup

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Run

```bash
uvicorn app.main:app --reload
```
