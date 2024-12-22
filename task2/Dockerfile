# Use the latest Ubuntu image as the base
FROM ubuntu:latest

# Update and upgrade the package manager
RUN apt-get update && apt-get upgrade -y

# Install Python3, pip3, and Flask
RUN apt-get install -y python3 python3-pip && \
    rm /usr/lib/python*/EXTERNALLY-MANAGED && \
    pip3 install flask

# Set the working directory to /app
WORKDIR /app

# Copy the Flask application to the Docker image
COPY ./api.py /app/api.py

# Expose port 5252 for the Flask server
EXPOSE 5252

# Define the command to run the Flask server
CMD ["python3", "api.py"]
