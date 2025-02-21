FROM ubuntu:22.04

# Set the working directory in the container
WORKDIR /app

# Copy the project files to the container
COPY . .

# Install Python and pip
RUN apt update && apt install -y python3 python3-pip

# Install required Python packages
RUN pip install django pillow

# Expose the default Django port (8000)
EXPOSE 8000

# Run Django's development server
CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]
