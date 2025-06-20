# FastAPI + Gunicorn + Nginx Demo (WSL)

This project demonstrates how to run a FastAPI app using Gunicorn (with Uvicorn workers) behind Nginx in a WSL environment.

## How to Run

1. Start FastAPI with Gunicorn:
```bash
gunicorn app.main:app -w 4 -k uvicorn.workers.UvicornWorker --bind 127.0.0.1:8000
