# Use an official Python runtime as a parent image
FROM python:2.7-slim

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install the required Python packages from requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Expose port 80
EXPOSE 80

# Define environment variable
ENV NAME World

# Run the app when the container starts
CMD ["python", "app.py"]
