# Python Testing with Pytest and Tox in Docker

This repository demonstrates a simple setup for testing Python code using Pytest and Tox within a Docker environment.

## Project Structure

```
.
├── Dockerfile           # Docker setup for Python environment
├── docker-compose.yml   # Docker Compose configuration
├── requirements.txt     # Python dependencies (Pytest and Tox)
├── main.py              # Main Python file with functions to test
├── test_main.py         # Pytest tests for the main.py functions
└── tox.ini              # Tox configuration for running tests in different environments
```

## Prerequisites
Make sure you have Docker and Docker Compose installed on your system.

* [Docker Installation Guide](https://docs.docker.com/engine/install/)

## Getting Started

### Clone the Repository
```
git clone https://github.com/yourusername/PyTestandTox.git
cd PyTestandTox
```

### Build the Docker Image
```
docker-compose build
```

### Run Tests with Tox
This command will run tests across all the Python environments specified in tox.ini.
```
docker-compose up
```

### Run Tests with Pytest Directly
If you prefer to run tests directly with Pytest:
```
docker-compose run pytest-tox pytest
```
