# Version-Docker-update
# StreamFlix Docker Project

This is a Dockerized Netflix-like website with three versions (v1, v2, v3).

## Project Overview

StreamFlix is a small streaming platform website that has been containerized using Docker. 
The project demonstrates how to maintain multiple versions of a website, run them simultaneously, and update the website efficiently using Docker.

## Problem Statement

- The website originally runs only on a single machine and cannot be easily shared.
- Updating the website requires manual changes and restarting the server, which is time-consuming.
- There is no version control for the deployed website.
- The website cannot scale to run multiple instances.

## Proposed Solution

- Package the website into Docker containers for consistent behavior on any machine.
- Maintain multiple versions (v1, v2, v3) as separate Docker images.
- Run multiple versions simultaneously on different ports.
- Make updates by modifying files, rebuilding the image, and running a new container.
- Optionally push Docker images to Docker Hub for sharing or cloud deployment.


docker build -t netflix-website:v1 .
docker run -d -p 8080:80 netflix-website:v1
