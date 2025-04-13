# Docker Nginx Static Site

A simple static website served using NGINX in a Docker container.

## Project Structure

docker-nginx-static-site/ ├── Dockerfile ├── index.html ├── README.md └── .gitignore

## Build the Docker Image

To build the Docker image for the static site, use the following command:

```bash
docker build -t docker-nginx-static-site .
Run the Container
To run the Docker container and expose the website on port 8080, use this command:
docker run -d -p 8080:80 docker-nginx-static-site
You can access the site at http://localhost:8080 or whichever port you mapped to.
Push to Docker Hub
1.Tag the image with your Docker Hub username:
docker tag docker-nginx-static-site your-dockerhub-username/docker-nginx-static-site
2.Push the image to Docker Hub:
docker push your-dockerhub-username/docker-nginx-static-site

Pull from Docker Hub (on another system)
To pull and run the image from Docker Hub on another system, use the following commands:
docker pull your-dockerhub-username/docker-nginx-static-site
docker run -d -p 8080:80 your-dockerhub-username/docker-nginx-static-site
Clean Up
To stop, remove containers, and clean up images:
docker ps -a       # List containers
docker stop <id>   # Stop a container
docker rm <id>     # Remove a container
docker rmi docker-nginx-static-site  # Remove image
Dependencies
Docker: Make sure you have Docker installed on your machine. If not, you can get it from Docker's official website.

You can paste this directly into your GitHub repository's `README.md` file. Let me know if you need any more edits!


