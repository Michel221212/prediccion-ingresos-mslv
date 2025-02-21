FROM python:3.11-slim-buster

WORKDIR /app/modelo

COPY . .

RUN pip install --no-cache-dir -r requirements.txt

CMD ["python", "train.py"]