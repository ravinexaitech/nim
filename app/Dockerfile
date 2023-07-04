FROM tiangolo/uvicorn-gunicorn-fastapi:python3.8

COPY ./app /app

# Install application dependencies
RUN pip install --no-cache-dir -r /app/requirements.txt

# Expose port 80
EXPOSE 80

# Start the application
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]
