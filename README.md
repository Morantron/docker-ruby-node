# Ruby + Nodejs Docker Image

This Docker image contains:
* The official docker image of ruby:2.3.5
* Nodejs 8.12.0
* Yarn 1.12.1

## Usage

Add `image: thylacinelol/docker-ruby-node` to your `bitbucket-pipelines.yml`

## Maintenance

- Update Dockerfile
- Build the image locally:
  ```
  docker build -t test_image .
  ```
- Run the test image and make sure everything is correct:
  ```
  docker run -i -t test_image:latest /bin/bash
  ```
- Login to docker
  ```
  docker login
  ```
- Build the release version (latest)
  ```
  docker build -t thylacinelol/docker-ruby-node:latest .
  ```
- Push the latest image to docker hub
  ```
  docker push thylacinelol/docker-ruby-node:latest
  ```
