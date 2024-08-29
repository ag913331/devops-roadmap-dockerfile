# Hello Captain Docker Project

## Description

This is a simple Docker project that prints "Hello, Captain!" to the console when the Docker container is run. The project demonstrates the creation of a Docker image using an Alpine Linux base image, and a single command to display a message before exiting.

## Dockerfile Explanation

The `Dockerfile` is straightforward and contains the following instructions:

- `FROM alpine:latest`: This line specifies the base image for the Docker container. We use the latest version of Alpine Linux, a lightweight Linux distribution perfect for small and efficient Docker images.

- `CMD ["echo", "Hello, Captain!"]`: This line sets the command to be executed when the Docker container is started. It runs the `echo` command, which prints "Hello, Captain!" to the console.

## Build and Use the Docker Image

Follow these steps to build and run the Docker image:

1. **Build the Docker Image**

   Navigate to the directory containing the `Dockerfile` and run the following command:
   ```bash
   docker build -t hello-captain .
   ```
This command builds the Docker image and tags it with the name `hello-captain`.

2. **Run the Docker Image**

   After building the image, you can run it using:
   ```bash
   docker run --rm hello-captain
   ```
This command runs the Docker container, which prints "Hello, Captain!" to the console. The `--rm` flag automatically removes the container after it exits.

## Project Structure

```text
.
├── Dockerfile
└── README.md
```
