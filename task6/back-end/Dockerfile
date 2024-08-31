# Use Ubuntu as the base image
FROM ubuntu:latest

# Install necessary packages and Python dependencies
RUN apt-get update && apt-get install -y python3 python3-pip

# Install Flask and Flask-CORS
RUN pip3 install flask flask-cors

# Set the working directory to /app
WORKDIR /app

# Copy the backend API code to /app
COPY ./api.py /app/api.py

# Expose port 5252
EXPOSE 5252

# Command to run the Flask API
CMD ["python3", "api.py"]
