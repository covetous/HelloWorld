# HelloWorld

A simple Hello World web application that displays a styled "Hello World" page, served via [nginx](https://nginx.org/) inside a Docker container.

## Project Structure

```
.
├── Dockerfile    # Docker image definition (nginx:alpine serving index.html)
├── index.html    # The Hello World front page
└── README.md     # Project documentation
```

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/) (for running with Docker)
- Any modern web browser (for running locally)

## Running with Docker

**Build the image:**

```bash
docker build -t helloworld .
```

**Run the container:**

```bash
docker run -p 8080:80 helloworld
```

**Open your browser and navigate to:**

```
http://localhost:8080
```

## Running Locally

Open `index.html` directly in your web browser — no server or build step required.

## What It Does

The application renders a centered "Hello World" heading on a light grey background. It is a minimal example demonstrating how to containerise a static HTML page with nginx and Docker.
