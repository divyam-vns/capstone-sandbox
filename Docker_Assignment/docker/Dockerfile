# docker/Dockerfile

# Step 1: Choose a base image
FROM python:3.10-slim

# Step 2: Set working directory
WORKDIR /app

# Step 3: Install system dependencies (example: wget, git)
RUN apt-get update && apt-get install -y \
    wget \
    git \
    && rm -rf /var/lib/apt/lists/*

# Step 4: Install Python packages
RUN pip install --no-cache-dir \
    numpy \
    pandas \
    matplotlib

# Step 5: Copy app code (if needed)
COPY . /app

# Step 6: Default command (optional)
CMD ["python3", "--version"]
