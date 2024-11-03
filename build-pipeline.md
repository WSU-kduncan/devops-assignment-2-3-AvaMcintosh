# DevOps Assigment 2 - GitHub Actions & DockerHub

## Description of Workflow
  - The trigger allows the workflow to run everytime there is a commit to main
    
  - Build Job - the job runs on the most recent ubuntu enviorment
  
  - Build Image Job
        - Downloads app.jar and Dockerfile
        - docker/setup-buildx-action@v2 - creates Docker Buildx
        - docker/login-action@v2 - logs into docker hub using DOCKERHUB_AVAMCINTOSH and DOCKERHUB_TOKEN
        - docker/build-push-action@v3 - builds the docker image and pushes it into the given repository avamcintosh520/mcintosh-wopro-service

## Link to DockerHub Repository
[DockerHub - `YOURLASTNAME-WOPro-Service`](https://hub.docker.com/r/avamcintosh520/mcintosh-wopro-service)

## Link to GitHub Actions Run Results Summary
[Link to **working** workflow run results](sampleURL:https://github.com/WSU-kduncan/s24cicd-pattonsgirl/actions/runs/8726150186/job/23941797523)
