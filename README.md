# Docker Static Website

## Overview

This project demonstrates how to deploy a static website using Docker and Nginx.

The application is containerized using Docker and served through an Nginx web server.

## Technologies Used

- Docker
- Nginx
- HTML

## Project Structure

```text
docker-static-website
│
├── Dockerfile
├── index.html
└── README.md
```

## Dockerfile

```dockerfile
FROM nginx:alpine

COPY index.html /usr/share/nginx/html/index.html

EXPOSE 80
```

## Build Docker Image

```bash
docker build -t akhil-nginx:v1 .
```

## Run Docker Container

```bash
docker run -d -p 8080:80 --name my-nginx akhil-nginx:v1
```

## Access Application

Open browser:

```text
http://localhost:8080
```

## Key Concepts Learned

- Docker Images
- Docker Containers
- Dockerfile
- Nginx
- Port Mapping
- Docker Volumes
- Docker Networking
- Multi-Stage Builds

## Future Improvements

- GitHub Actions CI/CD
- Docker Hub Integration
- Kubernetes Deployment
