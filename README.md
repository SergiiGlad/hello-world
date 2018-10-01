hello-world
===========

[![Deploy to Docker Cloud](https://files.cloud.docker.com/images/deploy-to-dockercloud.svg)](https://cloud.docker.com/stack/deploy/)

Sample docker image to test docker deployments

## Running locally

Build and run using Docker Compose:

	$ git clone https://github.com/docker/dockercloud-hello-world
	$ cd dockercloud-hello-world
	$ docker-compose up


## Deploying to Docker Cloud

[Install the Docker Cloud CLI](https://docs.docker.com/docker-cloud/tutorials/installing-cli/)

	$ docker login
	$ docker-cloud stack up

Hello world!

## Continuous Delivery Pipeline for Amazon ECS Using Jenkins, GitHub, and Amazon ECR
Make a change to a file in your repository, for example, readme.md, and push it to GitHub . If you configured things correctly, Jenkins pulls the code from your Git repository into a workspace, builds the container image, pushes the container image to ECR, creates a task and service definition, and starts your service.

The AWS documentation says: "If you have updated the Docker image of your application, you can create a new task definition with that image and deploy it to your service, one task at a time." This is pretty much everything that is currently available in the documentation currently (13th April 2015).
