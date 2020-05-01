# Docker image
FROM python:3

# Copy requirements
COPY requirements.txt /

# Install Requirements
RUN pip install -r /requirements.txt

# Copy scripts needed for execution
COPY . /usr/src/tc_demo2

# Establish a working directory
WORKDIR /usr/src/tc_demo2

# Execute required script
CMD ["python", "Car.py"] && CMD["pytest", "test_Car.py"]


