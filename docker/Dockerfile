# Use official Python image
FROM python:3.9-slim

# Set working directory inside container
WORKDIR /app

# Copy only requirements first (for caching)
COPY app/requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy full application code
COPY app/ .

# Expose Flask port
EXPOSE 5000

# Run the application
CMD ["python", "app.py"]