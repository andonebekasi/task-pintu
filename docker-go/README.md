#cicd build/push docker images to dockerhub (Sample apps GO)


# Build the Docker image:
Open a terminal, navigate to the webapp directory, and run the following command to build the Docker image:
docker build -t go-simple-web-static .

# Run the Docker container:
After the Docker image is built, you can run the container using the following command:
bash:
docker run -p 8080:8080 go-simple-web-static


## noted
change # Authenticate with Docker Hub

          - echo $DOCKERHUB_PASSWORD | docker login -u $DOCKERHUB_USERNAME --password-stdin


with your user and pass dockerhub


