# Use Python 3.10 as the base image
FROM public.ecr.aws/docker/library/python:3.10-slim-buster

# Set the working directory inside the container
WORKDIR /app

# Copy the contents of the current directory to /app in the container
COPY . /app

# Install dependencies from requirements.txt
RUN pip install --no-cache-dir -r /app/requirements.txt

# Expose port 5153
EXPOSE 5153

# Set an environment variable (if needed)
# ENV SOME_VARIABLE=value
ENV DB_USERNAME=myuser
ENV DB_PASSWORD=mypassword
ENV DB_HOST=127.0.0.1
ENV DB_PORT=5432
ENV DB_NAME=mydatabase
# Run the application when the container starts
CMD ["python", "app.py"]
