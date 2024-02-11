# Use an official Python runtime as the base image
FROM python:3

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any needed dependencies specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Make port 8080 available to the world outside this container
EXPOSE 8080

# Define environment variable
ENV CURRENT_ENVIRONMENT production

# Run app.py when the container launches
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0", "--port=8080"]  # Specify port 8080
