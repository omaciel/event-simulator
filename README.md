# Learn Kubernetes

## Building the image

  docker buildx build -t event-simulator:latest .

## Login to Quay.io

  docker login quay.io

## Run the image locally

  docker run -d event-simulator

## List the container

  docker ps -l

## Commit the image
Replace `74b076355784` with the value from the previous command:

  docker commit 74b076355784 quay.io/omaciel/learnkubernetes

## Push the image to Quay.io

  docker push quay.io/omaciel/learnkubernetes

## Pull the image from Quay.io

  docker pull quay.io/omaciel/event-simulator
