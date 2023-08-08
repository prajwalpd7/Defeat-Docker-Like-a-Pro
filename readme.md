# Docker Assignment
![Gif](https://miro.medium.com/v2/resize:fit:1400/0*bRvhcFgijNKRVD9L.gif)

## Objective:
Familiarize students with Docker fundamentals, container orchestration, multi-container apps, volume persistence, networking, and best practices to simulate real-world DevOps scenarios. 

## Prerequisite:
- Basic understanding of Docker.
- Docker installed on your local system.

## Task 1: Basic Docker Commands

1. **Pulling an Image**: Pull the official `nginx` image from Docker Hub.
2. **Running a Container**: Start an nginx container and expose it on port 8080.
3. **Inspecting Containers**: List all running containers, fetch details about a container.
4. **Interacting with Containers**: Log into the nginx container and install a text editor (e.g., vim).
5. **Stopping & Removing**: Stop the nginx container and then remove it.

## Task 2: Dockerfile Creation & Image Building

1. **Simple Dockerfile**: Create a Dockerfile to use `alpine` as a base and install `python3`.
2. **Optimized Dockerfile**: Optimize the above Dockerfile for caching (Hint: Consider the order of operations).
3. **Building an Image**: Use the Dockerfile to build an image.
4. **Running your Custom Image**: Start a container from the image you built.

## Task 3: Multi-container Application with Docker Compose

1. **Application Structure**: Create a simple web application that connects to a database (e.g., a Python Flask app with PostgreSQL).
2. **Docker Compose File**: Write a `docker-compose.yml` file to start your app and database in separate containers.
3. **Networking**: Ensure your web application can communicate with your database.
4. **Scaling with Compose**: Scale the web app to run 3 instances using Docker Compose.

## Task 4: Volumes & Persistent Data

1. **Bind Mounts**: Edit your web application live using bind mounts.
2. **Volume Creation**: Create a Docker volume and attach it to your PostgreSQL container.
3. **Data Persistence**: Test data persistence by stopping and restarting your containers.

## Task 5: Docker Networking

1. **Isolation**: Create two separate networks and ensure that containers from different networks cannot communicate with each other.
2. **Communication**: Set up a reverse proxy using nginx to route traffic to your web application.

## Task 6: Best Practices

1. **Security**: Use a non-root user in your Dockerfile.
2. **Efficiency**: Reduce the size of your images by using multi-stage builds.
3. **Logging**: Implement proper logging for your web application.

## Bonus Task: CI/CD Integration

1. **Pipeline**: Set up a simple CI/CD pipeline using a tool like Jenkins or GitHub Actions.
2. **Automate**: Automate the building of your Docker image when code is pushed to the repository.
3. **Deployment**: Extend the pipeline to automatically deploy (or update) your application using Docker Compose.

---

## Evaluation Criteria:

1. **Functionality**: Does the application run as expected with all services communicating effectively?
2. **Dockerfile & Compose Quality**: Are Dockerfiles and docker-compose files written optimally and efficiently?
3. **Understanding**: Can the student explain their choices and the Docker concepts behind the tasks they performed?
4. **Error Handling & Troubleshooting**: How does the student handle errors? Can they debug common container issues?

## Submission:

- Students should submit all Dockerfiles, scripts, and docker-compose files.
- A detailed report on the tasks completed, challenges faced, and how they overcame them.
