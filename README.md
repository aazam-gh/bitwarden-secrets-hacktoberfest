### Bitwarden Secrets Manager Hacktoberfest 2023

This is a Node.js REST API project that provides CRUD (Create, Read, Update, Delete) operations for tutorials. The project uses Express.js for the web server, MySQL for data storage, Docker for containerization, and Bitwarden Secrets Manager for securely storing MySQL database credentials.

## Features

- Create, Read, Update, and Delete tutorials.
- Securely store MySQL database credentials using Bitwarden Secrets Manager.
- Dockerized for easy deployment and environment consistency.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Docker installed.
- Bitwarden Secrets Manager setup with database credentials.


## Technical Details

The project can be run with the docker-compose.yaml file. The bitwarden subdirecotry has a Dockerfile for installing the bitwarden CLI. The docker-compose.yaml file mounts the bitwarden directory to the container and runs the bitwarden CLI to 
and retrive the secrets for the mysql user, password and database name.
The test-app directory contains the express app for creating the apis and a Dockerfile to build the image.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/your-nodejs-tutorials-api.git
    ```

2. Build the Docker image:

   ```bash
   docker compose up
   ```
