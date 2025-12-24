FROM python:3.12

COPY app.py /app.py
COPY requirements.txt /requirements.txt

RUN pip install --no-cache-dir --upgrade -r /requirements.txt

CMD ["sh", "-c", "uvicorn app:app --host 0.0.0.0 --port ${SERVER_PORT:-8000}"]
