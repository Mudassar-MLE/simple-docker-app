# simple-docker-app

A simple 'Hello World' application demonstrating the use of Docker containers. This project provides a basic example of containerizing an app using Docker.

## Project Structure:
```
simple-docker-app/
│
├── Dockerfile          # Contains the instructions to build the Docker image.
├── requirements.txt    # Python dependencies for the app.
├── main.py             # The main application code.
└── README.md           # Documentation for the project.
```


## Prerequisites

- [Docker](https://www.docker.com/get-started) installed on your system.
- A cloned copy of this repository.

## Getting Started

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Mudassar-MLE/simple-docker-app.git
   cd simple-docker-app
   code .
Note: You can use any code editor instead of vscode.

2. **Build the Docker image:**:
   ```bash
    docker build -t mudassar-mle/simple-docker-app:v1.0 .
This command builds the Docker image and tags it as mudassar-mle/simple-docker-app:v1.0

3. **Run the Docker container:**:
   ```bash
    docker run --rm -it -p 8001:8000 mudassar-mle/simple-docker-app:v1.0
This command builds the Docker image and tags it as mudassar-mle/simple-docker-app:v1.0

The `--rm` flag tells Docker to automatically remove the container when it exits.  
The `-it` flag runs the container in interactive mode.  
The `-p 8001:8000` option maps port `8000` inside the container to port `8001` on your local machine.

## Access the application:

Open your web browser and navigate to [http://localhost:8001](http://localhost:8001).  
You should see the message: `FastAPI Hello world! Version 1`.

## Test the `/test` endpoint:

Navigate to [http://localhost:8001/test](http://localhost:8001/test).  
You should see the message: `Testing hidden functionality ;)`.

## Author

- [@Muhammad Mudassar](https://github.com/Mudassar-MLE)
