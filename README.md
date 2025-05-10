# Docker_115


This is a Dockerized Django application, designed to provide a simple, containerized environment for running a Django project with a PostgreSQL database. It demonstrates how to set up a Django app, connect it to a PostgreSQL database, and run everything inside Docker containers.

## Features

- **Django**: Python web framework for rapid application development.
- **PostgreSQL**: Relational database used to store application data.
- **Docker**: Containerization for easy setup and deployment.

## Prerequisites

Before you begin, make sure you have the following installed:

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Getting Started

Follow these steps to get your project up and running locally:

1. Clone the Repository
git clone https://github.com/anageguchadze/Docker_115.git
cd Docker_115

2. Build and Run Containers
Run the following command to build the Docker image and start the containers:
docker-compose up --build
This will build the Docker image and start the containers (including the web app and PostgreSQL database).

3. Access the Django App
Once the containers are running, you can access the Django application by navigating to:
http://localhost:8000

4. Stop the Containers
To stop the containers, run:
docker-compose down

Development
For development purposes, any changes made to the code will automatically be reflected inside the container due to the volume mounting (./:/app).

1. Edit Code Locally
You can edit the code directly on your local machine, and changes will be reflected in the container.

2. Rebuild the Docker Container
If you make changes to dependencies or the Docker setup, rebuild the container:
docker-compose up --build

Notes
The application is using PostgreSQL as the database.
By default, Django runs in development mode (with debugging enabled). For production use, you may need to adjust settings in settings.py.

License
This project is licensed under the MIT License - see the LICENSE file for details.