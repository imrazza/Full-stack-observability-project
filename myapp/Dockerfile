FROM python:3.10

WORKDIR /app
COPY . .

RUN pip install fastapi uvicorn prometheus_client \
opentelemetry-api \
opentelemetry-sdk \
opentelemetry-exporter-otlp \
opentelemetry-instrumentation-fastapi

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
