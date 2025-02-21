FROM python:3.11-slim-buster

WORKDIR /app/api

# Copy the requirements file
COPY ../requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code
COPY .. .

# Expose the port that the app will listen on
EXPOSE 8000

# Run the API service using Uvicorn
CMD ["uvicorn", "api:app", "--host", "0.0.0.0", "--port", "8000"]