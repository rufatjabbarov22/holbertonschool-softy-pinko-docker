# Use the latest Ubuntu image as the base
FROM ubuntu:latest

# Update the APT package manager and upgrade installed packages
RUN apt-get update && apt-get upgrade -y

# Install Python 3 and pip 3
RUN apt-get install -y python3 python3-pip

# Fix the EXTERNALLY-MANAGED error if it occurs
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Set /app as the working directory
WORKDIR /app

# Copy the api.py file to /app directory in the container
COPY ./api.py /app/api.py

# Expose port 5252
EXPOSE 5252

# Run the Flask app
CMD ["python3", "api.py"]
