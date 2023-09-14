# firefox_inside_docker

# Docker Image for NewOS with Firefox

This repository provides a Docker image for NewOS with a pre-installed Firefox browser. You can use this image to easily run Firefox on your local system or anywhere else.

## Step 1: Create a Dockerfile

Start by creating a Dockerfile that describes how to build the Docker image. You can customize it as needed for your specific requirements.

## Step 2: Build the Docker Image

Build the Docker image using the following command. Replace `filename` with the name of your Dockerfile.
'''bash
docker build -t sachin5858/newos:v1 filename .

## Step 3: Push to Docker Hub
If you want to share your Docker image or use it on other systems, you can push it to Docker Hub. Make sure you're logged in to Docker Hub before running this command.

docker push sachin5858/newos:v1
Pull and Run the Docker Image Locally
To use the Docker image on your local system, follow these steps:

Pull the Docker image from Docker Hub:
docker pull sachin5858/newos:v1
Run the following command to start the container with Firefox:
docker run -it --rm --net=host --env="DISPLAY" --volume="$HOME/.Xauthority:/root/.Xauthority:rw" sachin5858/newos:v1

This will launch Firefox inside the container, and you can use it just like a regular browser.

## Step 4: Use Anywhere
You can now use the Docker image to launch Firefox anywhere you need it. Simply pull the image and run the container as shown in step 3.

Feel free to customize the Dockerfile and image as per your requirements.

Happy browsing!

