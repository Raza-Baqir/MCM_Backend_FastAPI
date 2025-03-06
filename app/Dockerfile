# Use Python base image
FROM python:3.10

# Set the working directory inside the container
WORKDIR /app

# Copy ALL files from project root to /app
COPY . .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose FastAPI port
EXPOSE 8000

# Command to run the FastAPI app
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
