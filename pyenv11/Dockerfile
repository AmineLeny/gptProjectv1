# Use an official Python runtime as a parent image
FROM python:3.12-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container
COPY . /app

# Update pip and install dependencies
RUN pip install --no-cache-dir --upgrade pip \
    && pip install --no-cache-dir --default-timeout=100 -r requirements.txt


# Make port 8000 available to the world outside this container
EXPOSE 8000

# Define environment variable
ENV OPENAI_API_KEY="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"

# Create the data directory
RUN mkdir -p /app/data

# Run queryGPT4.py when the container launches
CMD uvicorn querygpt4:app --host 0.0.0.0 --port 8000
