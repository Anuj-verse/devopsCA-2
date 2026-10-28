# Stage 3 — Fixed Dockerfile: slim base, non-root user, upgraded libs
FROM python:3.12-slim

WORKDIR /app

# Install requirements first so the install step is cached between builds
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy application code
COPY app.py .

# Create and switch to a non-root user
RUN addgroup --system appgroup && adduser --system --ingroup appgroup appuser
USER appuser

# Expose the backend port
EXPOSE 5000

# Start the app
CMD ["python", "app.py"]
