# Simple Python Flask Application

A simple Flask web application that returns "Hello, world!" when accessed.

## Files
- `app.py` - Main Flask application
- `requirements.txt` - Python dependencies (Flask)

## Local Setup (Before Docker)

### Prerequisites
- Python 3.8+
- pip

### Install dependencies
```bash
pip install -r requirements.txt
```

### Run the app locally
```bash
python app.py
```

Then open http://localhost:5000 in your browser.

## Docker Setup

### Build the Docker image
```bash
docker build -t simple-python-app:1.0 .
```

### Run the container
```bash
docker run -d -p 5000:5000 --name simple-python-app-container simple-python-app:1.0
```

### Access the application
Open http://localhost:5000 in your browser.

### Stop the container
```bash
docker stop simple-python-app-container
```

### Remove the container
```bash
docker rm simple-python-app-container
```
