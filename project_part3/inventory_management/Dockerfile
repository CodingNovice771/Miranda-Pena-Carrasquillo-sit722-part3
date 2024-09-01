# Dockerfile for inventory_management microservice
FROM python:3.9-slim

WORKDIR /app

COPY inventory_management/requirements.txt .

RUN pip install -r requirements.txt

COPY ./inventory_management/ .

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]
