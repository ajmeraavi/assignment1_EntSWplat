
# Use an official Python runtime as the base image
FROM python:3.8-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements file into the container
COPY requirements.txt .

# Install Flask and any other dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application into the container
COPY . .

# Make port  available to the host
EXPOSE 8080

# Define the command to run the Flask application
CMD ["python", "app.py"]
