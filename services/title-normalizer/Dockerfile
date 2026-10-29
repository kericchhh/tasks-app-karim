FROM python:3.12-slim

WORKDIR /title-normalizer

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY /app ./app

CMD ["flask", "--app", "app:create_app", "run", "--host=0.0.0.0", "--port=5001"]
