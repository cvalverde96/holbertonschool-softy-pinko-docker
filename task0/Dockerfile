# Is based on the latest ubuntu
FROM ubuntu:latest

# Update APT using apt-get update
RUN apt-get update

# Upgrade currently installed software through APT using apt-get upgrade -y
RUN apt-get upgrade -y

# Once built, you can run the Docker image in a container and it will echo “Hello, World!” on the terminal.
CMD echo "Hello, World!"

# commands to run for verification
# docker build -f ./Dockerfile -t softy-pinko:task0 . It creates a Docker image named softy-pinko with the version task0.
# docker run -it --rm --name softy-pinko-task0 softy-pinko:task0.  It starts a temporary container interactively, and the container is deleted after it stops.
