# Use an official Python runtime as a base image
FROM python:2.7-slim

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container ad /app
ADD . /app

# Install any need python packages specified in requirement.txt
RUN pip install -r requirements.txt

# Make paort 80 available to the world outside this container
EXPOSE 80

# Define enviroment variable
ENV NAME World

# Run the  app.py when the container launches
CMD ["python", "app.py"]
