# Demo App

Minimal FastAPI web app with a server-rendered HTML page and Docker support.

## Why FastAPI

FastAPI is the lighter option for this use case:

- minimal setup for a small app
- easy to serve HTML without a frontend build step
- straightforward Docker runtime with uvicorn on port 8000

## Run locally

```bash
pip install -r requirements.txt
uvicorn app.main:app --reload --port 8000
```

Open http://localhost:8000.

## Run with Docker

```bash
docker build -t demo-app .
docker run --rm -p 8000:8000 demo-app
```

Open http://localhost:8000.