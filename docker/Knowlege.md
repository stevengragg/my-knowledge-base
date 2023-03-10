# Docker


```ssh

# Build the app locally (assuming that you have a Dockerfile on root directory)

docker build -t <<proj-name>> .


# Run the app inside docker container locally

docker run -p 3000:3000 <<proj-name>>


```