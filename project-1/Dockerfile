# Use an official Python runtime as the base image
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements.txt file and install dependencies
COPY requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt

# Copy the entire source code into the container
COPY . /app/

# Expose port 5000 for the application (adjust as needed)
EXPOSE 5000

# Command to run the application
CMD ["python", "src/app.py"]
