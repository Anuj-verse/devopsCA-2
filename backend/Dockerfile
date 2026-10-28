# Stage 1 — Containerise the backend (python:3.9 as required by developers)
FROM python:3.9

WORKDIR /app

# Install requirements first so the install step is cached between builds
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy application code
COPY app.py .

# Expose the backend port
EXPOSE 5000

# Start the app
CMD ["python", "app.py"]
